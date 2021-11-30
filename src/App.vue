<template>
  <v-app>
    <navbar />

    <v-row class="mt-12">
      <v-col cols="6">
        <personal :estilo="'list-even'"  />
      </v-col>
      <v-col cols="6">
        <personal :estilo="'list-odd'" />
      </v-col>
    </v-row>

  <v-footer>
    <banner/>
  </v-footer>
  </v-app>
</template>

<script>
import navbar from "./components/navbar.vue";
import personal from "./components/personal.vue";
import banner from './components/banner.vue';

export default {
  components: { navbar, personal, banner },
  props:{
    estilo:String
  }
};
</script>

<style >
</style>