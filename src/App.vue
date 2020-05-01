<template>
  <v-app>
    <v-content>
      <Menu />
      <router-view />
    </v-content>
  </v-app>
</template>

<style lang="scss" scoped>
/* Large devices (laptops/desktops, 992px and up) */
@media screen and (min-width: 992px) {
  #app {
    padding-right: 56px;
    padding-left: 56px;
  }
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
