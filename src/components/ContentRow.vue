<template>
  <div
    class="d-inline-flex flex-column flex-sm-row align-center justify-center"
    :class="{ 'alternate-version': alternateVersion }"
  >
    <v-sheet class="content-row-image" :class="{ 'alternate-version-image': alternateVersion }">
      <v-img :src="require('@/assets/'+image)" />
    </v-sheet>
    <div
      class="content-row-text d-flex flex-column"
      :class="{ 'order-first': textFirst, 'alternate-version-text': alternateVersion }"
    >
      <h1 class="content-row-title title font-weight-bold">{{ title }}</h1>
      <p class="content-row-body body-2">{{ body }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.alternate-version {
  background-color: #213a25;
  .alternate-version-image {
    width: 100%;
  }
  .alternate-version-text {
    color: white;
    width: 100%;
  }
}

.content-row-image {
  width: 85%;
}
.content-row-text {
  width: 85%;
  padding: 24px 32px 8px 32px;

  .content-row-title {
    margin-bottom: 8px;
  }
}
/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
  .alternate-version {
    width: 100%;
    
    .alternate-version-image {
      width: 50%;
    }
    .alternate-version-text {
      width: 50%;
    }
  }

  .content-row-image {
    width: 50%;
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
}
/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}
/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
}
/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
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