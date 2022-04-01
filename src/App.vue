<template>
  <div>
    <div class="main">
      <h1>Component Styles</h1>
      <h4>Title of App.vue</h4>
      <Styles />
    </div>
  </div>
</template>

<script>
import Styles from "./components/Styles.vue";
export default {
  name: "App",
  components: {
    Styles,
  },
};
</script>

<style scoped>
body {
  background-color: rgb(115, 115, 226);
  text-align: center;
}
.main {
  margin-left: 0 auto;
}
h4 {
  color: orange;
  font-size: 1.4rem;
}
</style>
