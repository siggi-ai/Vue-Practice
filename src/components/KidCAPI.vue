<template>
  <div>
    <h4>Kid C</h4>
    <div>Name of the framework: {{ frameworkNameAPI }}</div>
  </div>
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
};
</script>