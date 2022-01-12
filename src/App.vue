<template>
  <div>
    <h1>Binding Classes</h1>
    <h2 class="underline" v-bind:class="state">Status</h2>
    <h3 v-bind:class="{ especially: 'IsEspecially' }">
      Ist dies ein besonderer Text
    </h3>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      state: "success",
      isEspecially: false,
    };
  },
};
</script>

<style scoped>
.underline {
  text-decoration: underline;
}
.especially {
  font-weight: 800;
  font-style: italic;
}
</style>
