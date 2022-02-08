<template>
  <div class="main">
    <h1>computed properties</h1>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: "Kunibert",
      lastName: "Winkelmann"
    };
  },
  computed : {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    }
  }
};
</script>

<style scoped>
.main {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
