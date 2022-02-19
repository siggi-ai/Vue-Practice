<template>
  <div>
    <h2>Herzlich Willkommen</h2>
    <h2 class="name">{{ firstName }}!</h2>
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
.name {
  color: lightcoral;
}
</style>
