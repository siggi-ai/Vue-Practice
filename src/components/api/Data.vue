<template>
  <h2>Alte Schreibweise:</h2>
  <h3>{{ firstName }}</h3>
  <h3>{{ lastName }}</h3>
  <h3>{{ club }}</h3>
</template>
<script>
export default {
  name: "Data",
  data() {
    return {
      firstName: "Klaus",
      lastName: "Strumm",
      club: "Peace Club",
    };
  },
};
</script>
