<template>
  <div class="home d-flex flex-column">
    <FullImageSheet image="header_photo.jpg">
      <v-img class="signature" src="@/assets/signature.png"/>
    </FullImageSheet>
    <ContentRow
      class="content-row-a"
      title="Explore the World"
      body="Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers. Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers. Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers."
      image="content_photo_1.jpg"
    />
    <ContentRow
      class="content-row-b"
      title="Explore the World"
      body="Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers."
      image="content_photo_1.jpg"
      text-first
      alternate-version
    />
    <ContentRow
      class="content-row-c"
      title="Explore the World"
      body="Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers."
      image="content_photo_1.jpg"
      text-first
    />
    <ContentRow
      class="content-row-d"
      title="Explore the World"
      body="Amazing tours and fun adventures are waiting for you. Treat yourself and see our offers."
      image="content_photo_1.jpg"
      alternate-version
    />
  </div>
</template>

<style lang="scss" scoped>
.content-row-a {
  margin-top: 64px;
  margin-bottom: 32px;
}
.content-row-b {
  margin-top: 32px;
  margin-bottom: 32px;
}
.content-row-c {
  margin-top: 32px;
  margin-bottom: 32px;
}
.content-row-d {
  margin-top: 32px;
  margin-bottom: 64px;
}
.signature {
  position: absolute;
  left: 0;
  bottom: 0;
  width: 15vw;
  filter: invert(100%);
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
