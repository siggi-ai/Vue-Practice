<template>
  <div>
    <h3>ProvideInjectAPI</h3>
    <KidA />
  </div>
</template>
<script>
import { provide } from "vue";
import KidA from "./KidAAPI.vue";
export default {
  name: "ProvideInjectAPI",
  //
  components: {
    KidA,
  },
  setup() {
    provide("frameworkNameAPI", "Vue 3");
  },
};
</script>
