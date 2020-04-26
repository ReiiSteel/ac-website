<template>
  <a class="link-icon" :href="link" target="_blank">
    <v-icon>{{ icon }}</v-icon>
  </a>
</template>

<style lang="scss" scoped>
.link-icon {
  padding: 8px;
}
</style>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "LinkIcon",
  props: {
    icon: String,
    link: String
  }
});
</script>