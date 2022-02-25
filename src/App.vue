<template>
  <div class="main">
    <h1>Components and v-model</h1>
    <Input v-model="name" />
    <div>eigegeben wurde {{ name }}</div>
  </div>
</template>

<script>
import Input from "./components/Input.vue";
export default {
  name: "App",
  components: {
    Input,
  },
  data() {
    return {
      name: "",
    };
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
