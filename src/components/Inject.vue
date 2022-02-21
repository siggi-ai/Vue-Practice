<template>
  <div>
    {{ userName }}
  </div>
</template>
<script>
export default {
  name: "Inject",
  inject: ["userName"],
};
</script>
<style scoped>
div {
  font-size: 30px;
}
</style>
