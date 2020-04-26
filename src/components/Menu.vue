<template>
  <v-sheet id="menu-sheet">
    <div class="title-section">
      <h1 class="display-1">Anne-Charlotte Mora</h1>
      <h2 class="subtitle-1 text-uppercase">Golfeuse professionnelle</h2>
    </div>
    <div class="menu-section">
      <v-tabs color="#2e7d32" centered>
        <v-tab>Accueil</v-tab>
        <v-tab>Birdie Fan-Club</v-tab>
        <v-tab>Partenaires</v-tab>
        <v-tab>Gallerie</v-tab>
      </v-tabs>
      <div class="social-media-bar">
        <LinkIcon icon="mdi-instagram" link="https://www.instagram.com/anne_chachaa/" />
        <LinkIcon
          icon="mdi-facebook"
          link="https://www.facebook.com/Anne-Charlotte-Mora-Golfeuse-Professionelle-111604830531361/"
        />
        <LinkIcon icon="mdi-twitter" link="https://twitter.com/anne_chachaa/" />
      </div>
    </div>
  </v-sheet>
</template>

<style lang="scss" scoped>
#menu-sheet {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  padding-top: 48px;
  padding-bottom: 32px;

  .title-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 24px;

    h2 {
      color: #00000059
    }
  }

  .menu-section {
    display: flex;
    flex-direction: column;
    align-content: center;

    .social-media-bar {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      align-self: center;
      width: 15vw;
    }
  }
}
</style>

<script lang="ts">
import Vue from "vue";
import LinkIcon from "@/components/LinkIcon.vue";

export default Vue.extend({
  name: "Menu",
  components: {
    LinkIcon
  }
});
</script>
