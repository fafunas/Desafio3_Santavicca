<template>
  <div id="App">
    <navbar class="p-2"/>
    <banner texto="Listado Personal"/>
    <personal/>
  </div>
</template>

<script>
import navbar from './components/navbar.vue'
import banner from './components/banner.vue'
import personal from './components/personal.vue'

export default {
  name: 'App',
  components: {
    navbar,
    banner,
    personal
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
