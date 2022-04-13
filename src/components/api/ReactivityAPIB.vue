<template>
  <div>
    <h2>{{ state.firstName }} {{ state.lastName }}</h2>
  </div>
</template>
<script>
import { reactive } from "vue";
export default {
  name: "ReactivityAPIA",
  setup() {
    const state = reactive({
      firstName: "Angela",
      lastName: "Merkel",
    });
    return {
      state,
    };
  },
};
</script>