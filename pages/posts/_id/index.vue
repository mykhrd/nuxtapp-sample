<template>
  <div class="post">
      <section class="post--section">
          <h1 class="post--title">title of posts</h1>
          <div class="post--details">
              <div>last updated on xx-xxx-xxx </div>
              <div>written by xxxxx</div>
          </div>
          <p class="post--content">content of the post</p>
      </section>
    <section class="post--feedback">
        <p>test</p>
    </section>
  </div>
</template>
<style scoped>
.post {
  max-width: 95%;
  padding: 20px;
  width: 100%;
}
.post--section {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;

  padding: 20px;
}
.post--feedback {
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;

  border-top: 2px solid gray;
  padding: 20px;
}
</style>
