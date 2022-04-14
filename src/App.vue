<template>
  <div>
    <h1>Methods</h1>
    <div class="blogCreate main">
      <Methods />
      <MethodsAPIRef />
      <MethodsAPIReactive />
    </div>
  </div>
</template>

<script>
import Methods from "./components/api/Methods.vue";
import MethodsAPIRef from "./components/api/MethodsAPIRef.vue";
import MethodsAPIReactive from "./components/api/MethodsAPIReactive.vue";

export default {
  name: "App",
  components: {
    Methods,
    MethodsAPIRef,
    MethodsAPIReactive,
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
