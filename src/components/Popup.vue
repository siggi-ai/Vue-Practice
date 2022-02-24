<template>
  <div>
    <h2>Popup.vue</h2>
    <h2>hier poppt die Nachricht auf :)</h2>
    <button v-on:click="$emit('close', name)">Popup schließen</button>
    <input
      type="text"
      id="name"
      v-model="name"
      placeholder="Name"
      class="input"
    />
    ">
  </div>
</template>
<script>
export default {
  name: "Popup,",
  data() {
    return {
      name: "",
    };
  },
  emits: {
    close: (name) => {
      if (!name) {
        return false;
      } else {
        return true;
      }
    },
  },
};
</script>
