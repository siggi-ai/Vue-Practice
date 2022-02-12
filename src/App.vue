<template>
  <div class="main">
    <h1>computed properties</h1>
    <h2>{{ fullName }} {{ title }}</h2>
    <h3>
      There once was a person called {{ fullName }}, who was called
      {{ title }} by everyone. She lived in a great {{ home }} and ate
      a lot of {{ food }}.
    </h3>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: "Cat",
      lastName: "Power",
      title: "the Greatest",
      home: "castle",
      food: "pizza",
    };
  },
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    },
  },
};
</script>

<style scoped>
.main {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(115, 115, 226);
}
</style>
