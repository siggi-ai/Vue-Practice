<template>
  <div class="main">
    <h1>Cigarettes</h1>
    <h2 class="underline" v-bind:class="state">Status</h2>
    <h3 v-bind:class="active ? 'especially' : 'normal'">
      Ist dies ein besonderer Text
    </h3>
    <h4
      v-bind:class="{
        underline: true,
        especially_bold: active && IsBold,
        especially: active && !IsBold,
        only_bold: !IsEspecially && IsBold
      }"
    >
      Ein Array mit mehreren Klassen
    </h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      state: "success",
      active: true,
      isBold: true,
    };
  },
};
</script>

<style scoped>
.main {
  background-color: #000;
  color: white;
  padding: 10px;
  font-family:Georgia, 'Times New Roman', Times, serif;
}
.underline {
  text-decoration: underline;
}
.especially {
  font-weight: 800;
  font-style: italic;
}
.especially_bold {
  font-weight: 800;
  color: orange;
  font-style: italic;
}
.only_bold {
  font-weight: 800;
}
.normal {
  color: aqua;
}
</style>
