<template>
  <div class="main">
    <h1>List Rendering</h1>
    <h2 v-for="(fullName, index) in fullNames" :key="index">
      {{ fullName.name }}, {{ fullName.description }}</h2>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      fullNames: [
        { name: "Hans", description: "Engineer" },
        { name: "Gabi", description: "Politician" },
        { name: "Melanie", description: "Author" },
      ],
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
