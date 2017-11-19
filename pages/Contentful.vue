<template>
<v-layout>
    <h1>{{ title }}</h1>
    <h3>{{ person.fields.name }}</h3>
    <!-- render blog posts -->
    <template v-for="post in posts">
      <h3>{{ post.fields.title }}</h3>
      <p>{{post.fields.description}}</p>
      <hr>
    </template>
    <br>
    <hr>
    <hr>
    <br>
    <!-- <section v-for="post in posts">
            <template v-for="(val,key) in post">
              <li>{{key}}: {{val}}</li>
              <br>
            </template>
            <hr>
          </section> -->
    <!-- <section v-for="post in posts">
      <div v-for="fields in post">
        <ul v-for="(val,key) in fields">
          <li>{{key}}: {{val}}</li>
        </ul>
      </div>
      <hr>
    </section> -->
</v-layout>
</template>

<script>
  import {createClient} from '~/plugins/contentful.js'

  const client = createClient()

  export default {
    data () {
      return {
        title: 'Contentful works!'
      }
    },
    // `env` is available in the context object
    asyncData ({env}) {
      return Promise.all([
        // fetch the owner of the blog
        client.getEntries({
          'sys.id': env.CTF_PERSON_ID
        }),
        // fetch all blog posts sorted by creation date
        client.getEntries({
          'content_type': env.CTF_BLOG_POST_TYPE_ID,
          order: '-sys.createdAt'
        })
      ]).then(([entries, posts]) => {
        // return data that should be available
        // in the template
        return {
          person: entries.items[0],
          posts: posts.items
        }
      }).catch(console.error)
    }
  }
</script>
