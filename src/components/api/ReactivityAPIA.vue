<template>
  <div>
    <h2>{{ framework }}</h2>
  </div>
</template>
<script>
import { ref } from "vue";
export default {
  name: "ReactivityAPIA",
  setup() {
    let framework = ref("Vue 2");
    setTimeout(() => {
      framework.value = "vue 3";
      console.log("new framework:", framework);
    }, 2000);
    return {
      framework,
    };
  },
};
</script>
