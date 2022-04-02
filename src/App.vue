<template>
  <div>
    <div class="main">
      <h1>HTTP</h1>
      <Suggestions />
      <br />
    </div>
    <div class="blogCreate main">
      <BlogCreate />
    </div>
  </div>
</template>

<script>
import BlogCreate from "./components/BlogCreate.vue";
import Suggestions from "./components/Suggestions.vue";

export default {
  name: "App",
  components: {
    BlogCreate,
    Suggestions,
  },
};
</script>

<style scoped>
body {
  background-color: rgb(115, 115, 226);
}
.main {
  text-align: center;
  margin-left: 0 auto;
  padding: 30px;
  font-size: 1rem;
  margin: 0 auto;
  width: 500px;
  font-family: "Courier New", Courier, monospace;
}
.blogCreate {
  width: 240px;
  text-align: ;
}
</style>
