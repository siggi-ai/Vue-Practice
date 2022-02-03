<template>
  <div class="text">
    <h1>Computed Properties</h1>
    <h4>
      Bundesligaspiele Summe:
      {{
        players.reduce(
          (total, current) => (total = total + current.numberofMatches),
          0
        )
      }}
    </h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      players: {
        id: 1,
        firstName: "Klaus",
        lastName: "Fischer",
        club: "FC Schalke 04",
        numberOfMatches: 535,
      },
    };
  },
  computed: {
    fullName() {
      return `${this.form.firstName} ${this.form.lastName}`;
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
