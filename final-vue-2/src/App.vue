<template>
  <!--
  <saludo person="Cachichurris" heroe="Pirulin"/>
  <saludo />
  <articlee/>
  <articlee title="Mataron a San Juan" :likes="50" :isPublished="false"/>-->
  <button @click="showPopup = true">Mostrar el fricking popup</button>
  <popup v-show="showPopup" @close="showPopup = false"/>

</template>


<script>
/* eslint-disable vue/no-unused-components */

import popup from './components/popup.vue'
import articlee from './components/articlee.vue'
import saludo from './components/saludo.vue'
export default { 
  name: 'App',
  components: {
    articlee,
    saludo,
    popup
  },
  data(){
    return {
      showPopup: false
    }
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
