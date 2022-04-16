<template>
  <div>
    <label for="firstName">
      <span>Vorname</span>
    </label>
    <input
      type="text"
      id="firstName"
      v-model="firstName"
      placeholder="Vorname"
    />
    <label for="lastName">
      <span>Nachname</span>
    </label>
    <input
      type="text"
      id="lastName"
      v-model="lastName"
      placeholder="Nachname"
    />
    <h2>Hello {{ fullName }} !</h2>
  </div>
</template>
<script>
export default {
  name: "Computed",
  data() {
    return {
      firstName: "",
      lastName: "",
    };
  },
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    },
  },
};
</script>