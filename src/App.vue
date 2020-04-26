<template>
  <v-app>
    <v-content>
      <Menu/>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import Menu from './components/Menu.vue';

export default Vue.extend({
  name: 'App',

  components: {
    Menu
  },

  data: () => ({
    //
  }),
});
</script>
