<template>
  <h2>Neue Schreibweise: {{ firstName }}</h2>
</template>
<script>
import { ref } from "vue";
export default {
  name: "DataAPI",
  setup() {
    const firstName = ref("Klaus");
    return {
      firstName: firstName,
    };
  },
};
</script>
