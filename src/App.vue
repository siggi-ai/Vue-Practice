<template>
  <div>
    <h1>replacing data with ref</h1>
    <div class="blogCreate main">
      <Data />
    </div>
    <div class="blogCreate main">
      <DataAPI />
    </div>
  </div>
</template>

<script>
import Data from "./components/api/Data.vue";
import DataAPI from "./components/api/DataAPI.vue";

export default {
  name: "App",
  components: {
    Data,
    DataAPI,
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
