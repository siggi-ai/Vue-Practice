<template>
  <div class="main">
    <h1>Conditional List Rendering</h1>

    <template v-for="name in names" :key="name">
      <h3 v-if="name === 'Annalena'">{{ name }}</h3>
    </template>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      names: ["Angela", "Armin", "Annalena", "Olaf"],
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
