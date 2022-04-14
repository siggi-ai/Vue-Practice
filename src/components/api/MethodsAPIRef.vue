<template>
  <div>
    <h2>Neue Schreibweise</h2>
    <h3>{{ firstName }} {{ lastName }}</h3>
    <h4>{{ goals }}</h4>
    <button v-on:click.prevent="changeName">Namen ändern</button>
    <button v-on:click.prevent="newGoal">Tor erzielt</button>
  </div>
</template>
<script>
import { ref } from "vue";
export default {
  name: "MethodsAPIRef",
  setup() {
    const firstName = ref("Gerd");
    const lastName = ref("Hamm");
    const goals = ref(0);

    function changeName() {
      this.firstName = "Siegfried";
      this.lastName = "Choi";
    }
    function newGoal() {
      goals.value++;
    }
    return {
      firstName,
      lastName,
      goals,
      changeName,
      newGoal,
    };
  },
};
</script>
