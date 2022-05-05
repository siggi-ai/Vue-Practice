<template>
  <div>
    <h1>Lifecycle Hooks (Composition API)</h1>
    <div class="blogCreate main">
      <h4>Alte Schreibweise</h4>
      <Lifecycle />
    </div>
    <div class="blogCreate main">
      <h4>Composition API</h4>
      <LifecycleAPI />
    </div>
  </div>
</template>

<script>
import Lifecycle from "./components/Lifecycle.vue";
import LifecycleAPI from "./components/LifecycleAPI";

export default {
  name: "App",
  components: {
    Lifecycle,
    LifecycleAPI,
  },
};
</script>

<style>
body {
  background-color: rgb(117, 117, 255);
  font-family: "Courier New", Courier, monospace;
}
h1 {
  margin: 0 auto;
  margin-top: 50px;
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
