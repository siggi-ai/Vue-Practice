<template>
  <div class="main">
    <h1>Conditional Rendering</h1>
    <div v-show="display">offensichtlich ist display true</div>
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
