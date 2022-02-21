<template>
  <h2>Spielbericht</h2>
  <div v-bind="$attrs">child komponente ohne root-element</div>
</template>
<script>
export default {
  name: "Spielbericht",
};
</script>