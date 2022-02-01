<template>
  <div>
    <h1>Modifiers</h1>
    <h2>Eingabebereich</h2>
    <form v-on:submit="submitForm">
      <div>
        <div>
          <label for="age">
            <span>Alter in Jahren</span>
          </label>
          <input type="text" id="age" v-model="form.age" />
        </div>
      </div>
    </form>
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
  display: flex;
}
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}

input {
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
