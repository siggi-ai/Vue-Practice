<template>
  <div class="main">
    <h1>List Rendering</h1>
    <h2 v-for="name in names" :key="name">{{ name }}</h2>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      names: ["Hans", "Gabi", "Peter"],
    };
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
