<template>
  <v-sheet class="full-img-sheet">
    <v-img :src="require('@/assets/'+image)">
      <slot />
    </v-img>
  </v-sheet>
</template>

<style lang="scss" scoped>
.full-img-sheet {
  width: 100%;
}
</style>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";

const FullImageSheetProps = Vue.extend({
  props: {
    image: String
  }
});

@Component
export default class FullImageSheet extends FullImageSheetProps {}
</script>