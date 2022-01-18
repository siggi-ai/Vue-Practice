<template>
  <div class="main">
    <h1>Methods</h1>
    <h4>Summe von 1 + 2 + 3 + 4 + 5 + 6 = {{ add(1, 2, 3, 4, 5, 6) }}</h4>
    <h4>Summe von 1 + 2 + 3 + 5 + 8 + 13 = {{ add(1, 2, 3, 5, 8, 13) }}</h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {};
  },
  methods: {
    add(a, b, c, d, e, f,) {
      return a + b + c + d + e + f;
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
