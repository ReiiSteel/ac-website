<template>
  <v-sheet class="full-img-sheet">
    <v-img src="../assets/header_photo.jpg"></v-img>
  </v-sheet>
</template>

<style lang="scss" scoped>
.full-img-sheet {
  
    padding-top: 30px;
    padding-bottom: 30px;
    padding-right: 50px;
    padding-left: 50px;
  
}
</style>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "FullImageSheet"
});
</script>