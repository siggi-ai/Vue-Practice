<template>
  <div>
    <h2>Neue Schreibweise mit Reactive</h2>
    <h3>{{ firstName }} {{ lastName }}</h3>
    <h4>{{ goals }}</h4>
    <button v-on:click.prevent="changeName">Namen ändern</button>
    <button v-on:click.prevent="newGoal">Tor erzielt</button>
  </div>
</template>
<script>
import { reactive, toRefs } from "vue";
export default {
  name: "MethodsAPIReactive",
  setup() {
    const state = reactive({
      firstName: "Gerd",
      lastName: "Hamm",
      goals: 0,
    });

    function changeName() {
      this.firstName = "Siegfried";
      this.lastName = "Choi";
    }
    function newGoal() {
      state.goals++;
    }
    return {
      ...toRefs(state),
      changeName,
      newGoal,
    };
  },
};
</script>
