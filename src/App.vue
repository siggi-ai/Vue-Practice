<template>
  <div class="text">
    <h1>Computed Properties</h1>
    <div>{{ form.firstName }} {{ form.lastName }}</div>
    <div>Name mit Computed Property: {{ fullName }}</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      form: {
        firstName: "Angela",
        lastName: "Merkel",
      },
    };
  },
  computed: {
    fullName() {
      return `${this.form.firstName} ${this.form.lastName}`;
    }
  }
};
</script>

<style scoped>
.text {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
