<template>
    <div>
        <h1>sample single user</h1>
        <p>user ID: {{ $route.params.id }}</p>
    </div>
</template>
<script>
export default {
  // validate
  validate(data) {
    console.log(data)
    // validate value
    // return data.params.id == 1

    // regex
    return /^\d+$/.test(data.params.id)
  }
}
</script>
