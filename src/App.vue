<template>
  <div>
    <h1>Template Refs</h1>
    <div class="blogCreate main">
      <BlogList />
    </div>
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

<style>
body {
  background-color: rgb(115, 115, 226);
  font-family: "Courier New", Courier, monospace;
}
.main {
  text-align: center;
  margin-left: 0 auto;
  padding: 30px;
  font-size: 1rem;
  margin: 0 auto;
  width: 500px;
  font-family: "Courier New", Courier, monospace;
  color: #000;
}
.blogCreate {
  width: 240px;
  text-align: center;
}
</style>
