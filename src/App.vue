<template>
  <div>
    <h1>Mixins</h1>
    <div class="blogCreate main">
      <CounterByHover />
      <CounterByClick />
    </div>
  </div>
</template>

<script>
import CounterByHover from "./components/CounterByHover.vue";
import CounterByClick from "./components/CounterByClick.vue";

export default {
  name: "App",
  components: {
    CounterByHover,
    CounterByClick,
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
