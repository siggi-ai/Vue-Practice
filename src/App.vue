<template>
  <div class="main">
    <h1>List Rendering</h1>
    <template v-for="(fullName, index) in fullNames" :key="index">
      <h2>
        {{ fullName.name }}, {{ fullName.description }}, {{ fullName.age }}
      </h2>
      <h4 v-for="(character, index) in fullName.characters" :key="index">
        {{ character }}
      </h4>
      <br>
    </template>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      fullNames: [
        {
          name: "Hans",
          description: "Engineer",
          age: 32,
          characters: ["cool", "reliable", "fancy"],
        },
        {
          name: "Gabi",
          description: "Politician",
          age: 42,
          characters: ["eloquent", "intelligent", "greedy"],
        },
        {
          name: "Melanie",
          description: "Author",
          age: 29,
          characters: ["playful", "creative", "unreliable"],
        },
      ],
      fullPlaces: [
        { name: "Hamburg", description: "Northern Germany" },
        { name: "Berlin", description: "East Germany" },
        { name: "Munich", description: "South Germany" },
      ],
    };
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
