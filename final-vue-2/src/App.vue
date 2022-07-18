<template>
  
  <saludo person="Cachichurris" heroe="Pirulin"/>
  <saludo />
  <articlee/>
  <articlee title="Mataron a San Juan" :likes="50" :isPublished="false"/>

</template>


<script>
/* eslint-disable vue/no-unused-components */

import articlee from './components/articlee.vue'
import saludo from './components/saludo.vue'
export default { 
  name: 'App',
  components: {
    articlee,
    saludo,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
