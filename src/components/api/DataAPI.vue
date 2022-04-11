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
    const lastName = ref("Müller");
    const club = ref("Bayern München");
    firstName.value = "Angela";
    const greeting = `Hallo ${firstName.value} ${lastName.value} ($club.value)`;
    console.log("firstName: ", firstName);
    return {
      firstName,
      lastName,
      club,
      greeting,
    };
  },
};
</script>
