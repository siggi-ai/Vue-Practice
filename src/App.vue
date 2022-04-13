<template>
  <div>
    <h1>Reactivity</h1>
    <div class="blogCreate main">
      <ReactivityAPIA />
    </div>
  </div>
</template>

<script>
import ReactivityAPIA from "./components/api/ReactivityAPIA.vue"

export default {
  name: "App",
  components: {
    ReactivityAPIA,
  },
};
</script>

<style>
body {
  background-color: rgb(153, 153, 255);
  font-family: "Courier New", Courier, monospace;
}
h1 {
  margin: 0 auto;
  width: 200px;
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
