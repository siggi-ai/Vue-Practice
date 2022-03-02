<template>
  <div>
    <h3 v-for="player in players" :key="player.lastName">
      <slot></slot>
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
        {
          firstName: "Eggbert",
          lastName: "Hahn",
          age: 19,
        },
      ],
    };
  },
};
</script>
