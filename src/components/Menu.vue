<template>
  <v-sheet id="menu-sheet">
    <h1>Anne-Charlotte Mora</h1>
    <h2>Golfeuse professionnelle</h2>
    <v-tabs color="#2e7d32" centered>
      <v-tab>Accueil</v-tab>
      <v-tab>Birdie Fan-Club</v-tab>
      <v-tab>Partenaires</v-tab>
      <v-tab>Gallerie</v-tab>
    </v-tabs>
  </v-sheet>
</template>

<style lang="scss" scoped>
#menu-sheet {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
</style>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Menu"
});
</script>
