<template>
  <div class="text">
    <h1>Computed Properties</h1>
    <h4>
      Bundesligaspiele Summe:
      {{ sumNumberOfMatches }}
    </h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
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
  computed: {
    sumNumberOfMatches() {
      return this.players.reduce(
        (total, current) => (total = total + current.numberOfMatches), 0
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
