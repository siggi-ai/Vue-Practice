<template>
  <div class="text">
    <h1>Computed Properties</h1>
    <template v-for="players in players" :key="players.id">
      <div v-if="players.numberOfMatches > 500">
        {{ players.firstName }} {{ players.lastName }} {{ players.club }} hat
        insgesamt {{ players.numberOfMatches }} Bundesligaspiele absolviert.
      </div>
    </template>
    <button
      v-on:click="
        players.push({
          id: 4,
          firstName: 'Hannes',
          lastName: 'Fischer',
          club: 'FC Schalke 04',
          numberOfMatches: 189,
        })
      "
    >
      Mit Hannes
    </button>
    <h4>
      Bundesligaspiele Summe:
      {{ sumNumberOfMatches }}
    </h4>
    <h4>
      Bundesligaspiele Summe (methods):
      {{ getSumNumberOfMatches() }}
    </h4>
    <div>
      <label class="label">
        <span class="label-text" for="color">Farbe</span>
      </label>
      <input type="text" id="color" v-model="color" class="input" />
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      color: "",
      players: [
        {
          id: 1,
          firstName: "Klaus",
          lastName: "Fischer",
          club: "FC Schalke 04",
          numberOfMatches: 535,
        },
        {
          id: 2,
          firstName: "Norbert",
          lastName: "Nigbur",
          club: "FC Schalke 04",
          numberOfMatches: 456,
        },
        {
          id: 3,
          firstName: "Norbert",
          lastName: "Fichtel",
          club: "FC Schalke 04",
          numberOfMatches: 552,
        },
      ],
    };
  },
  methods: {
    getSumNumberOfMatches() {
      console.log("methods getSumNumberOfMatches");
      return this.players.reduce(
        (total, current) => (total = total + current.numberOfMatches),
        0
      );
    },
  },
  computed: {
    sumNumberOfMatches() {
      console.log("computed sumNumberOfMatches");
      return this.players.reduce(
        (total, current) => (total = total + current.numberOfMatches),
        0
      );
    },
  },
};
</script>

<style scoped>
.text {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
