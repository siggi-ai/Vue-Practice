<template>
  <div class="main">
    <h1>Binding Styles</h1>
    <div
      v-bind:style="{
        color: highlightColor,
        'font-size': divSize + 'px',
      }"
    >
      Inline Stlye
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      highlightColor: "#4FC08D",
      divSize: "50",
    };
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
.underline {
  text-decoration: underline;
}
</style>
