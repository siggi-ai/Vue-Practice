<template>
  <div class="main">
    <h1>Binding Styles</h1>
    <div v-bind:style="divStyleObject">Inline Stlye</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      divStyleObject: {
        color: "orange",
        fontSize: "50px",
        padding: "2px",
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
.underline {
  text-decoration: underline;
}
</style>
