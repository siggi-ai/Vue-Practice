<template>
  <div class="main">
    <div>
      <h1>Provide and Inject</h1>
    </div>

    <Inject />
  </div>
</template>

<script>
import Inject from "./components/Inject.vue";
export default {
  name: "App",
  components: {
    Inject,
  },
  data() {
    return {};
  },
};
</script>

<style>
body {
  background-color: rgb(115, 115, 226);
  display: flex;
  text-align: center;
}

.main {
  padding: 100px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(150 150 240);
}

.pic {
  display: flex;
  float: right;
}
</style>
