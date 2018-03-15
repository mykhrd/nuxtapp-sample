<template>
  <section class="container">
    <div class="wrap">
      <a href="/users">normal_link users</a>
    </div>
    <div class="wrap">
       <nuxt-link to="/users">nuxt_link users</nuxt-link>
    </div>
    <div class="wrap">
        <button @click="loadProductPage">product page</button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    loadProductPage() {
      this.$router.push("/products/")
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
}
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
.wrap {
  margin: 10px;
}
</style>
