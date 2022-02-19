<template>
  <div class="main">
    <h1>first child</h1>
    <Hallo />
  </div>
</template>

<script>
import Willkommen from './components/Willkommen.vue';
export default {
  name: "App",
  components: {
    Hallo: Willkommen
  }
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
