<template>
  <v-layout column justify-center>
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

    <ninjas></ninjas>
    <!-- <contentful v-bind:person="cPerson" v-bind:posts="cPosts"></contentful> -->

    <transition name="ballmove" enter-active-class="rollIn" leave-active-class="rollOut">
    <h2>this transitions in</h2>
    </transition>
    <transition appear-to-class="rollIn">
    <h2>this transitions in</h2>
    </transition>

    <!-- <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse, iusto, quisquam ipsam possimus expedita perspiciatis adipisci est quas ipsum id minima. Fugit deleniti nam quod quia architecto exercitationem maxime, rerum laudantium sapiente quisquam adipisci nesciunt pariatur corporis odio similique vel impedit reiciendis voluptatem ipsam doloribus minima quaerat delectus veniam? Modi minus maxime <br><br>que quaerat eligendi doloribus esse quisquam ratione, accusamus <br><br> dicta soluta magnam delectus. Saepe quos non ut facilis ipsam doloribus earum modi at aliquid quasi autem, numquam voluptatem deleniti fugiat, ea atque a rerum esse suscipit accusamus. In impedit, illum non nostrum neque nisi. Sapiente nam iure at quidem pariatur quaerat repellendus quos facilis aliquam, debitis consequuntur odit quia quibusdam. Dignissimos numquam maiores, eum doloribus alias neque voluptatem id dolorum nihil soluta ut suscipit nesciunt commodi natus sed, hic ab fugiat provident praesentium dolor quasi. Nulla blanditiis at laborum vel accusamus, consectetur similique sint asperiores aperiam quod voluptatem culpa rem voluptas ea unde voluptatibus excepturi! Similique ratione optio architecto soluta impedit debitis officia adipisci iure hic voluptatem? Enim dolorum deleniti alias, quos eaque labore provident, minus commodi placeat ipsa, sit culpa tempora aspernatur accusamus aliquam iste dignissimos eligendi saepe aliquid magni corporis! Enim quam voluptates exercitationem inventore nobis eveniet fugit dicta vero perferendis facere maxime magnam consequuntur, dignissimos amet minus deserunt aut ipsum reprehenderit voluptatibus illum unde dolore laboriosam <br><br> cupiditate! Inventore ab iste itaque veniam iusto tenetur ipsam rem, dignissimos repellendus accusantium. Dolore quo vel possimus nobis nesciunt iure cum praesentium dolorum, corporis qui similique nemo, magnam reiciendis enim necessitatibus tenetur rem officiis quaerat est fuga neque sed. Aliquam officia pariatur sint aperiam? Beatae, voluptatem placeat? Rem tempore debitis nobis officiis omnis odit tempora nisi? Beatae ipsam dolores magni et blanditiis perferendis velit placeat rerum ipsum. Provident impedit animi ipsum rerum voluptate non fugit excepturi eaque iste mollitia repudiandae quo odit cum, natus soluta sequi iure ex <br><br>que. Excepturi quo velit praesentium non minima similique libero autem aut voluptates dolores molestias, unde, enim quaerat at provident! Aspernatur laudantium mollitia sed rerum, sint architecto suscipit, optio itaque inventore, repellat ex consectetur hic temporibus. Animi sequi quis dicta aspernatur <br><br>que sunt id omnis qui similique eius. Consequuntur assumenda, dolore fuga quia iusto quasi sed inventore rem in? Expedita, architecto natus veniam quis, consectetur error cum enim nemo nam alias ipsa ipsum inventore perspiciatis earum tempore ratione praesentium neque iure possimus dolore, laboriosam commodi quod debitis! Eius et commodi dolores nisi praesentium, aspernatur eligendi soluta facilis, ratione quod veniam ipsa itaque corporis, ex neque. Placeat voluptatibus voluptate veritatis, quas fugit similique dolor tempora laborum, eos delectus temporibus ad quam magni praesentium ducimus eius accusamus exercitationem unde distinctio incidunt. Rerum nulla eos eius, incidunt soluta iusto in obcaecati cum dolorum vero quas aliquid, nisi sint hic facere neque provident voluptatibus vitae sed aliquam ducimus dolores temporibus culpa. Error nihil hic, molestias ut distinctio, minima fuga, asperiores accusamus sit esse saepe temporibus aperiam ducimus veritatis! Accusantium nesciunt rem est earum. Amet itaque culpa dolores tempore sequi quo error exercitationem. Voluptates a perferendis reprehenderit! Culpa commodi, atque eius, exercitationem aliquid expedita nemo quod sequi sint sunt illum cupiditate porro laudantium! Corrupti praesentium fugit doloribus itaque alias rem. Mollitia adipisci voluptatem est veritatis voluptatibus enim nobis aliquid voluptas sint quisquam maiores, culpa nostrum quam eligendi corrupti labore! Obcaecati perferendis molestiae incidunt recusandae. Suscipit, vel. Totam, quae ipsam nobis dolor reiciendis impedit eligendi? Sequi cupiditate mollitia quaerat distinctio reprehenderit. Fuga rem temporibus corporis ullam cumque? Necessitatibus error unde harum corporis ipsam voluptate assumenda beatae quisquam sunt voluptatem, enim in ullam cum excepturi impedit veniam expedita aspernatur quia, minus, soluta perferendis! Debitis id quia, magnam iste dolore veniam consequuntur architecto eveniet vel amet ut tenetur ipsa quod. Ullam ducimus dolorum suscipit quibusdam aut mollitia deserunt quam! Consectetur qui ad, debitis repellendus alias facere laudantium aperiam explicabo quidem! Praesentium nemo quo quod commodi. Officiis consectetur, facilis ipsam enim sed architecto dolores unde voluptatum illo, porro minus nulla excepturi fuga molestiae error placeat sunt sit labore suscipit reiciendis odit saepe beatae! Fugiat, reprehenderit! Expedita nemo distinctio nostrum mollitia fuga dignissimos ducimus iusto. Est officiis, voluptatem rerum placeat aliquid cumque dolor exercitationem laborum qui quibusdam consequatur eveniet aperiam corporis voluptatum, assumenda quae mollitia at, error modi aut. Alias deserunt dignissimos nisi, sunt corrupti impedit fugit quam ipsa possimus quae quasi architecto quidem cumque, necessitatibus perferendis adipisci dolorum! Unde eligendi incidunt iure, dicta <br><br> nobis tempore dolor necessitatibus at officiis. Architecto maiores vero explicabo accusantium ipsa et, qui placeat ut. Cumque natus dolores quasi omnis, incidunt sint iusto tenetur nulla in. Iure libero quas esse fugiat fugit quae voluptatem voluptatum repudiandae <br><br>que quasi! Fuga aut quos in autem cum expedita sunt eaque tempora nemo laborum deleniti ab non tempore unde explicabo accusamus odit suscipit, quae neque nulla id alias tenetur laboriosam! Dicta dignissimos quae eum possimus quam laudantium, quod nesciunt.</p> -->
  </v-layout>
</template>

<style>
.rollIn{
  transform: translate3d(0, 400px 0);
}
.rollOut{
  transform: translate3d(0, -400px 0);
}
</style>


<script>
import Ninjas from '../components/Ninjas'
import Contentful from './Contentful'
export default {
  components: {
    'ninjas': Ninjas,
    'contentful': Contentful
  }
}
</script>
