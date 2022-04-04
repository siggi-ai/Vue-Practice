<template>
  <div>
    <h1>Lifecycle Hooks</h1>
    <div class="blogCreate main">
      <Parent />
    </div>
  </div>
</template>

<script>
import Parent from "./components/Parent.vue";

export default {
  name: "App",
  components: {
    Parent,
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
