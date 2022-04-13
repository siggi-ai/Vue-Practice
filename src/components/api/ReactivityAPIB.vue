<template>
  <div>
    <h2>{{ firstName }} {{ lastName }}</h2>
  </div>
</template>
<script>
import { reactive } from "vue";
export default {
  name: "ReactivityAPIA",
  setup() {
    const state = reactive({
      firstName: "Angelo",
      lastName: "Bildani",
    });
    setTimeout(() => {
      (state.firstName = "Heino"),
        (state.lastName = "Jäger"),
        console.log("new state:", state);
    }, 2000);
    return {
      firstName: state.firstName,
      lastName: state.lastName,
    };
  },
};
</script>