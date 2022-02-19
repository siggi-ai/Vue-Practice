<template>
  <div>
    <h2>Herzlich Willkommen {{ firstName }}!</h2>
  </div>
</template>
<script>
export default {
  name: "Willkommen",
  props: {
    firstName: String,
  },
};
</script>

<style scoped>
h2 {
    color: #0032a1;
}
</style>
