<template>
  <h2>Neue Schreibweise:</h2>
  <h3>{{ state.firstName }}</h3>
  <h3>{{ state.lastName }}</h3>
  <h3>{{ state.club }}</h3>
  <p>{{ greeting }}</p>
  <p>{{ introduction }}</p>
</template>
<script>
import { reactive } from "vue";
export default {
  name: "DataAPI",
  setup() {
    const state = reactive ({
      firstName: "Fritz",
      lastName: "Müller",
      club: "Red Hat Club",
      hobby: "sailing",
    });
    const greeting = `Hallo ${state.firstName} ${state.lastName} (${state.club})`;
    const introduction = `I am ${state.firstName} and I like ${state.hobby}!`;
    return {
      state,
      greeting,
      introduction,
    };
  },
};
</script>
