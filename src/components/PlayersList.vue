<template>
  <div>
    <h3 v-for="player in players" :key="player.lastName">
      {{ player.firstName }} {{ player.lastName }} {{ player.age }}
    </h3>
  </div>
</template>
<script>
export default {
  name: "PlayersList",
  data() {
    return {
      players: [
        {
          firstName: "Klaus",
          lastName: "Fischer",
          age: 21,
        },
        {
          firstName: "Klaus",
          lastName: "Fichtel",
          age: 22,
        },
        {
          firstName: "Norbert",
          lastName: "Nigur",
          age: 22,
        },
      ],
    };
  },
};
</script>
