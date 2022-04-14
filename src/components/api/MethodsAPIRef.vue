<template>
  <div>
    <h2>Alte Schreibweise</h2>
    <h3>{{ firstName }} {{ lastName }}</h3>
    <h4>{{ goals }}</h4>
    <button v-on:click.prevent="changeName">Namen ändern</button>
    <button v-on:click.prevent="newGoal">Tor erzielt</button>
  </div>
</template>
<script>
export default {
  name: "Methods",
  data() {
    return {
      firstName: "Gerd",
      lastName: "Hamm",
      goals: 0,
    };
  },
  methods: {
    changeName() {
      this.firstName = "Siegfried";
    },
    newGoal() {
      this.goals++;
    },
  },
};
</script>
