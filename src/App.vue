<template>
  <v-app>
    <v-content>
      <Menu />
      <router-view />
    </v-content>
  </v-app>
</template>

<style lang="scss" scoped>
#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

<script lang="ts">
import Vue from "vue";
import Menu from "@/components/Menu.vue";

export default Vue.extend({
  name: "App",

  components: {
    Menu
  },

  data: () => ({
    //
  })
});
</script>
