<template>
      <div>
        <!-- <h1>sample single user</h1>
        <p>user ID: {{ $route.params.id }}</p> 
        -->
        <input type="text" v-model="userId">
        <button @click="onLoadUser">get user</button>
        <nuxt-child/>
    </div>
</template>
<script>
export default {
  data() {
    return {
      userId: ""
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push("/users/" + this.userId)
    }
  }
}
</script>
