<template>
  <div>
    <h1>v-model & Composition API</h1>
    <div class="blogCreate main">
      <h4>AlteSchreibweise</h4>
      <VModel />
      <h4>Compostion API mit Ref</h4>
      <VModelAPIRef />
      <h4>Composition API mit Reactive</h4>
      <VModelAPIReactive />
    </div>
  </div>
</template>

<script>
import VModel from "./components/api/VModelAPIReactive.vue";
import VModelAPIRef from "./components/api/VModelAPIRef.vue";
import VModelAPIReactive from "./components/api/VModelAPIReactive.vue";

export default {
  name: "App",
  components: {
    VModel,
    VModelAPIRef,
    VModelAPIReactive,
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
