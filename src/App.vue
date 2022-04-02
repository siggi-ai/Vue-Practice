<template>
  <div class="main">
    <h1>HTTP</h1>
    <BlogList />
  </div>
</template>

<script>
import BlogList from "./components/BlogList.vue";

export default {
  name: "App",
  components: {
    BlogList,
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
  font-size: 2rem;
  margin: 0 auto;
  width: 500px;
  font-family: 'Courier New', Courier, monospace;
}
</style>
