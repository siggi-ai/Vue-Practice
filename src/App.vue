<template>
  <div class="main">
    <h1>Methods</h1>
    <h4>Summe von 1 + 2 + 3 + 4 + 5 + 6 = {{ add() }}</h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {};
  },
  methods: {
    add() {
      return 1 + 2 + 3 + 4 + 5 + 6;
    },
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
