<template>
  <div class="main">
    <h1>Form Handling</h1>
    <label class="label" for="firstName">
      <span class="label-text">Vorname</span>
    </label>
    <input 
      type="text"
      id="firstname"
      v-model="form.firstName"
      placeholder="Vorname"
      class="input input-bordered">
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: 0,
      name: "Hanni",
    };
  },
  methods: {
    changeCount(value, event) {
      console.log("event: ", event)
      this.count = this.count + value;
    },
    changeName(event) {
      console.log("changeName: ", event);
      this.name = "Bernd";
    },
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
