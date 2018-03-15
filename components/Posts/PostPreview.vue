<template>
  <div class="post">
    <nuxt-link :to="'posts/' + id">
        <article class="post-article">
          <div class="post-thumb" :style="{backgroundImage: 'url(' + thumbnail + ')' }"></div>
          <div class="post-content">
            <h1 class="post-title">{{ title }}</h1>
            <p>{{ previewText }}</p>
          </div>
        </article>
      </nuxt-link>
  </div>
</template>

<script>
export default {
  name: "PostPreview",
  props: {
    id: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    previewText: {
      type: String,
      required: true
    },
    thumbnail: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.post {
  border: 1px solid gray;
  padding: 10px;
}
.post:hover {
  opacity: 0.5;
}

.page--top {
  text-align: center;
}

.post-thumb {
  background: #999;
  background-size: cover;
  background-position: center;
  height: 200px;
}
</style>
