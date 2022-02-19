<template>
  <div class="main">
    <h1>first child</h1>
    <Willkommen />
    <Willkommen />
    <Willkommen />
  </div>
</template>

<script>
import Willkommen from "./components/Willkommen.vue";
export default {
  name: "App",
  components: {
    Willkommen,
  },
};
</script>

<style scoped>
.main {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(115, 115, 226);
}
</style>
