<template>
  <div class="d-inline-flex align-center" :class="{ 'alternate-version': alternateVersion }">
    <v-sheet class="content-row-image" :class="{ 'alternate-version-image': alternateVersion }">
      <v-img :src="require('@/assets/'+image)" />
    </v-sheet>
    <div
      class="content-row-text d-flex flex-column"
      :class="{ 'order-first': textFirst, 'alternate-version-text': alternateVersion }"
    >
      <h1 class="content-row-title d-title font-weight-bold">{{ title }}</h1>
      <p class="content-row-body body-2">{{ body }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.alternate-version {
  width: 100%;
  background-color: #213a25;
  .alternate-version-image {
    width: 50% !important;
  }
  .alternate-version-text {
    width: 50% !important;
    color: white;
  }
}

.content-row-image {
  width: 35%;
}
.content-row-text {
  width: 30%;
  padding: 32px;

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
    title: {
      type: String,
      required: true
    },
    body: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    textFirst: {
      type: Boolean,
      default: false
    },
    alternateVersion: {
      type: Boolean,
      default: false
    }
  }
});

@Component
export default class ContentRow extends ContentRowProps {}
</script>