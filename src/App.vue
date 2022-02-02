<template>
  <div>
    <h1>Modifiers</h1>
    <h2>Eingabebereich</h2>
    <form v-on:submit.prevent="submitForm">
      <div>
        <label for="age">
          <span>Alter in Jahren</span>
        </label>
        <br />
        <input type="text" id="age" v-model.number.lazy="form.age" />
      </div>
      <button>Daten übermitteln</button>
    </form>
    <h2>Ausgangsbereich</h2>
    <div v-for="(item, key, index) in form" :key="index">
      {{ key }}: {{ item }}
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      form: {
        age: null,
      },
    };
  },
  methods: {
    submitForm(event) {
      event.preventDefault();
      console.log("Form data: ", this.form);
    },
  },
};
</script>

<style scoped>
body {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
