<template>
  <div class="main">
    <h1>Binding Styles</h1>
    <div v-bind:style="[baseStyleObject, successStyleObject]">Inline Stlye</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      baseStyleObject: {
        fontSize: "20px",
        padding: "2px",
      },
      successStyleObject: {
        color: "green",
        backgroundColor: "lightblue",
        border: "1 px solid",
      }
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
