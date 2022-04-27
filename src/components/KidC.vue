<template>
  <div>
    <h4>Kid C</h4>
    <div>Name of the framework: {{ frameworkName }}</div>
  </div>
</template>
<script>
export default {
  name: "KidC",
  inject: ["frameworkName"],
};
</script>