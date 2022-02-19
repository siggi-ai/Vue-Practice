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
