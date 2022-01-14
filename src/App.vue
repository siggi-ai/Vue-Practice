<template>
  <div class="main">
    <h1>Conditional Rendering</h1>
    <template v-if="display === true">
      <h2>VUE 3</h2>
      <h2>VSC</h2>
      <h2>HCS</h2>
    </template>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      display: true,
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
