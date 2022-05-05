<template>
  <div>
    <h5>Lifecycle Hooks in Lifecycle</h5>
  </div>
</template>
<script>
export default {
  name: "Lifecycle",
  //
  //
  beforeCreate() {
    console.log("Lifecycle beforeCreate");
  },
  created() {
    console.log("Lifecycle created");
  },
  beforeMount() {
    console.log("Lifecycle beforeMount");
  },
  mounted() {
    console.log("Lifecycle mounted");
  },
  beforeUpdate() {
    console.log("Lifecycle beforeUpdate");
  },
  updated() {
    console.log("Lifecycle updated");
  },
  beforeUnmount() {
    console.log("Lifecycle beforeUnmount");
  },
  unmounted() {
    console.log("Lifecycle unmounted");
  },
};
</script>