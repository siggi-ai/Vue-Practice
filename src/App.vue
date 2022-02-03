<template>
  <div>
    <h1>v-pre</h1>
    <div v-pre>
      {{ form.firstName }}
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      form: {
        firstName: "Angela",
      },
    };
  },
};
</script>

<style scoped>
body {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
