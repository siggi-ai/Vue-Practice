<template>
  <div>
    <h1>Computed Properties & Composition API</h1>
    <div class="blogCreate main">
      <h4>AlteSchreibweise</h4>
      <Computed />
      <h4>Compostion API mit Ref</h4>
      <ComputedAPIRef />
      <h4>Composition API mit Reactive</h4>
      <ComputedAPIReactive />
    </div>
  </div>
</template>

<script>
import Computed from "./components/api/Computed.vue";
import ComputedAPIRef from "./components/api/ComputedAPIRef.vue";
import ComputedAPIReactive from "./components/api/ComputedAPIReactive.vue";

export default {
  name: "App",
  components: {
    Computed,
    ComputedAPIRef,
    ComputedAPIReactive,
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
