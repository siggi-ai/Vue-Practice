<template>
  <div class="main">
    <h1>Lists and Keys</h1>
    <div v-for="name in names" :key="name">
      <h3>{{ name }}</h3>
      <input placeholder="Nachname" />
    </div>
    <button class="button" v-on:click="changeOrder">Liste neu sortieren</button>
  </div>
</template>

<script>
import _ from "lodash";
export default {
  name: "App",
  data() {
    return {
      names: ["Angela", "Armin", "Annalena", "Olaf"],
    };
  },
  methods: {
    changeOrder() {
      console.log(this.names);
      this.names = _.shuffle(this.names);
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
