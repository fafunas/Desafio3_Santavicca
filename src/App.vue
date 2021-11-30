<template>
  <div id="App">
    <navbar class="p-2"/>
    <banner texto="Listado Personal"/>
    <personal :estilo="'list-even'" :personas="personas"/>
    <hr>
    <personal :estilo="'list-odd'" :personas="personas"/>
  </div>
</template>

<script>
import personas from './assets/data/personas.json'
import navbar from './components/navbar.vue'
import banner from './components/banner.vue'
import personal from './components/personal.vue'

export default {
  name: 'App',
  components: {
    navbar,
    banner,
    personal
  },
  data() {
    return {
      personas
      
    }
  },
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
