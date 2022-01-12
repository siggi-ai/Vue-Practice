<template>
  <div class="main">
    <h1>Cigarettes</h1>
    <h2 class="underline" v-bind:class="state">Status</h2>
    <h3 :class="{ especially: active }">Ist dies ein besonderer Text</h3>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      state: "success",
      active: true,
    };
  },
};
</script>

<style scoped>
.main {
  background-color: #000;
  color: white;
  padding: 10px;
  font-family: Arial, Helvetica, sans-serif;
}
.underline {
  text-decoration: underline;
}
.especially {
  font-weight: 800;
  font-style: italic;
}
</style>
