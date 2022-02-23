<template>
  <div>
    <h2>Popup.vue</h2>
    <h2>hier poppt die Nachricht auf :)</h2>
    <button v-on:click="$emit('close')">Popup schließen</button>
  </div>
</template>
<script>
export default {
  name: "Popup,",
};
</script>
