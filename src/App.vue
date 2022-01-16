<template>
  <div class="main">
    <h1>List Rendering</h1>
    <h2 v-for="(fullName, index) in fullNames" :key="index">
      {{ fullName.name }}, {{ fullName.description }}, {{ fullName.age }}</h2>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      fullNames: [
        { name: "Hans", description: "Engineer", age: 32 },
        { name: "Gabi", description: "Politician", age: 42 },
        { name: "Melanie", description: "Author", age: 29 },
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
