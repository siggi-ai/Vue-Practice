<template>
  <div class="main">
    <h2>Eingabebereich</h2>
    <form action="">
      <div>
        <h1>Form Handling</h1>
        <label class="label" for="firstName">
          <span class="label-text">Vorname</span>
        </label>
        <input
          type="text"
          id="firstname"
          v-model="form.firstName"
          placeholder="Vorname"
          class="input input-bordered"
        />
        <div>
          <label class="label" for="lastName">
            <span class="label-text">Nachname</span>
          </label>
          <input
            type="text"
            id="lastname"
            v-model="form.lastName"
            placeholder="Nachname"
            class="input input-bordered"
          />
        </div>
      </div>
    </form>
    <h2>Ausgabebereich</h2>
    <div>
      <div v-for="(item, key, index) in form" :key="index">
        {{ key }}: {{ item }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
