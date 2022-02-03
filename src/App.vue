<template>
  <div>
    <h1>v-pre</h1>
    <div v-once>
      <input type="text" id="firstName" v-model="form.firstName" />
    </div>
    <button v-on:click="form.firstName = 'Annalena'">Namen ändern</button>
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
