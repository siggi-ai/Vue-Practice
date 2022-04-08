<template>
  <h2>Neue Schreibweise: {{ firstName }}</h2>
  <p>{{ greeting }}</p>
</template>
<script>
import { ref } from "vue";
export default {
  name: "DataAPI",
  setup() {
    const firstName = ref("Klaus");
    firstName.value = "Angela";
    const greeting = `Hallo ${firstName.value}`;
    console.log("firstName: ", firstName);
    return {
      firstName,
      greeting,
    };
  },
};
</script>
