<template>
  <div>
    <h4>Kid C</h4>
    <div>Name of the framework: {{ frameworkNameAPI }}</div>
  </div>
  <h1>{{ message }}</h1>
</template>
<script>
import { inject } from "vue";
export default {
  name: "KidCAPI",
  //
  setup() {
    const frameworkNameAPI = inject("frameworkNameAPI", "Default framework");
    //
    return {
      frameworkNameAPI,
    };
  },
  inject: ["message"],
  created() {
    console.log(this.message); // injected value
  },
};
</script>