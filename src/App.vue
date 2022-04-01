<template>
  <div>
    <h1>Component Styles</h1>
    <h4>Title of App.vue</h4>
    <Styles />
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
  display: flex;
  text-align: center;
}
h4 {
  color: orange;
  font-size: 1.4rem;
}
</style>
