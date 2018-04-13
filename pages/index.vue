<template>
  <div class="page--top">
    <section class="intro">
      <h1>section1</h1>
      <p>intro</p>
    </section>
    <section>
      <PostPreview id="1" thumbnail="//images.pexels.com/photos/34600/pexels-photo.jpg" title="hello there!" previewText="First post!" />
      <PostPreview id="1" thumbnail="//images.pexels.com/photos/270366/pexels-photo-270366.jpeg" title="hello there!" previewText="second post!" />
      <PostPreview id="1" thumbnail="//images.pexels.com/photos/34600/pexels-photo.jpg" title="hello there!" previewText="third post!" />
    </section>
  </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview"

export default {
  components: {
    PostPreview
  }
}
</script>

<style scoped>

</style>
