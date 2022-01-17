<template>
  <div class="main">
    <h1>List Rendering</h1>
    <template v-for="(item, key, index) in fullNames" :key="key">
      <h3>{{ key }}: {{ item }} ({{ index }})</h3>
    </template>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      fullNames: {
        name: "Franz",
        description: "Engineer",
        age: 32,
      },
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
