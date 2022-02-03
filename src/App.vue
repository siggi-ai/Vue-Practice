<template>
  <div class="text">
    <h1>Computed Properties</h1>
    <div>{{ form.firstName }} {{ form.lastName }}</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      form: {
        firstName: "Angela",
        lastName: "Merkel"
      },
    };
  },
};
</script>

<style scoped>
.text {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
