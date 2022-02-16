<template>
  <div class="main">
    <h1>Watchers</h1>
    <h2>{{ fullName }}</h2>
  </div>
  <div>
    <button v-on:click="changeFullName">neuer Name</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: "Clara",
      lastName: "Fall",
    };
  },
  methods: {
    changeFullName() {
      this.fullName = "Hansi Hinterseer";
    },
  },
  computed: {
    fullName: {
      get() {
        return `${this.firstName} ${this.lastName}`;
      },
      set(value) {
        const names = value.split(" ");
        this.firstName = names[0];
        this.lastName = names[1];
      },
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
