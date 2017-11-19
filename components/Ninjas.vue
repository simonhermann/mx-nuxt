<template>
    <div>
      <h3>{{ title }}</h3>
      <ul>
        <li v-for="ninja in ninjas" v-on:click="ninja.show = !ninja.show">
          <b>{{ ninja.name }}</b> : 
          <span v-show="ninja.show">{{ ninja.speciality }}</span>
        </li>
      </ul>
    </div>
</template>

<style scoped>
h3 {
  color: purple;
}
</style>


<script>
export default {
  data () {
    return {
      title: 'Ninja App',
      ninjas: [
        {name: 'Ryu', speciality: 'Vue Components', show: false},
        {name: 'Crystal', speciality: 'Click events', show: false},
        {name: 'Tangi', speciality: 'Webpack', show: false}
      ]
    }
  }
}
</script>
