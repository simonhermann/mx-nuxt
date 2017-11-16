<template>
  <v-layout column justify-center align-center>
    <!-- <v-flex xs12 sm8 md6>
      <div class="text-xs-center">
        <img src="/v.png" alt="Vuetify.js" class="mb-5" />
      </div>
      <v-card>
        <v-card-title class="headline">Welcome to the Vuetify + Nuxt.js template</v-card-title>
        <v-card-text>
          <p>Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.</p>
          <p>For more information on Vuetify, check out the <a href="https://vuetifyjs.com" target="_blank">documentation</a>.</p>
          <p>If you have questions, please join the official <a href="https://chat.vuetifyjs.com/" target="_blank" title="chat">discord</a>.</p>
          <p>Find a bug? Report it on the github <a href="https://github.com/vuetifyjs/vuetify/issues" target="_blank" title="contribute">issue board</a>.</p>
          <p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
          <div class="text-xs-right">
            <em><small>&mdash; John Leider</small></em>
          </div>
          <hr class="my-3">
          <a href="https://nuxtjs.org/" target="_blank">Nuxt Documentation</a>
          <br>
          <a href="https://github.com/nuxt/nuxt.js" target="_blank">Nuxt GitHub</a>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="primary" flat nuxt to="/inspire">Continue</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex> -->

      <h1>{{ person.fields.name }}</h1>
      <!-- render blog posts -->
      <ul>
        <li v-for="post in posts">
          {{ post.fields.title }}
        </li>
      </ul>
      
  </v-layout>
</template>


<script>
  import {createClient} from '~/plugins/contentful.js'

  const client = createClient()

  export default {
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
