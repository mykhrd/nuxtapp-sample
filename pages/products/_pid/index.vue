<!-- 
dynamic path
-->
<template>
    <div>
        <h1>single product page</h1>
        <p>product ID: {{ $route.params.pid }}</p>
        <button @click="getDetails">get details</button>
    </div>
</template>
<script>
export default {
  data() {
    return {
      pId: ""
    }
  },
  methods: {
    getDetails() {
      this.$router.push("/products/" + this.$route.params.pid + "/details/")
    }
  }
}
</script>