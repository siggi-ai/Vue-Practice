<template>
  <div>
    <h3>ProvideInject: {{ framework }}</h3>
    <KidA />
  </div>
</template>
<script>
import KidA from "./KidA.vue";
export default {
  name: "ProvideInject",
  //
  components: {
    KidA,
  },
  data() {
    return {
      framework: "Vue3",
    };
  },
  provide() {
    return {
      frameworkName: this.framework,
    };
  },
};
</script>
