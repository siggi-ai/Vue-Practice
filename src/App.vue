<template>
  <div>
    <h1>Template Refs</h1>
    <div class="blogCreate main">
      <TemplateRef />
    </div>
  </div>
</template>

<script>
import TemplateRef from "./components/TemplateRef.vue";

export default {
  name: "App",
  components: {
    TemplateRef,
  },
};
</script>

<style>
body {
  background-color: rgb(153, 153, 255);
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
