<template>
  <div>
    <h1>Watch & Composition API</h1>
    <div class="blogCreate main">
      <h4>AlteSchreibweise</h4>
      <Watch />
      <h4>Compostion API mit Ref</h4>
      <WatchAPIRef />
      <h4>Composition API mit Reactive</h4>
      <WatchAPIReactive />
    </div>
  </div>
</template>

<script>
import Watch from "./components/api/Watch.vue";
import WatchAPIRef from "./components/api/WatchAPIRef.vue";
import WatchAPIReactive from "./components/api/WatchAPIReactive.vue";

export default {
  name: "App",
  components: {
    Watch,
    WatchAPIRef,
    WatchAPIReactive,
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
