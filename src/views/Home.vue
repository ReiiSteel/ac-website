<template>
  <div class="home d-flex flex-column">
    <div>
      <FullImageSheet class="header-image" image="header_photo.jpg" />
    </div>
    <ContentRow
      class="content-row-a align-self-center"
      title="Explore the World"
      body="Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers."
      image="content_photo_1.jpg"
    />
  </div>
</template>

<style lang="scss" scoped>
.content-row-a {
  margin-top: 128px;
  margin-bottom: 128px;
}
</style>

<script>
// @ is an alias to /src
import FullImageSheet from "@/components/FullImageSheet";
import ContentRow from "@/components/ContentRow";

export default {
  name: "Home",
  components: {
    FullImageSheet,
    ContentRow
  }
};
</script>
