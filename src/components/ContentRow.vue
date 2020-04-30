<template>
  <div class="d-inline-flex align-center">
    <v-sheet class="content-row-image">
      <v-img :src="require('@/assets/'+image)" />
    </v-sheet>
    <div class="content-row-text d-flex flex-column">
      <h1 class="content-row-title title font-weight-bold">{{ title }}</h1>
      <p class="content-row-body body-2">{{ body }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.content-row-image {
  width: 35vw;
}
.content-row-text {
  width: 30vw;
  padding: 24px;

  .content-row-title {
    letter-spacing: 2px !important;
    margin-bottom: 24px;
  }

  .content-row-body {
    text-align: justify;
  }
}
</style>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";

const ContentRowProps = Vue.extend({
  props: {
    title: String,
    body: String,
    image: String
  }
});

@Component
export default class ContentRow extends ContentRowProps {}
</script>