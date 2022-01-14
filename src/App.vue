<template>
  <div class="main">
    <h1>Conditional Rendering</h1>
    <h2 v-if="display === true">VUE 3</h2>
    <h2 v-if="display === true">VSC</h2>
    <h2 v-if="display === true">HCS</h2>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      display: true
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
