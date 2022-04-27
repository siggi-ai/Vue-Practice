<template>
  <div>
    <h4>KidC</h4>
    <div>Name of the framework: {{ frameworkName }}</div>
  </div>
</template>
<script>
export default {
  name: "KidC",
  inject: ["frameworkName"],
};
</script>