<template>
  <div class="main">
    <h1>Watchers</h1>
    <h2>Immediate and Deep</h2>
    <div>
      <span>Radiosender</span>
      <input type="text" v-model="radiosender" />
    </div>
    <div>
      <span>Webadresse:</span>
      <input type="text" v-model="senderInfo.web">
    </div>
    <div>
      <span>gegründet am:</span>
      <input type="text" v-model="senderInfo.web">
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      radiosender: "Eins LIVE",
    };
  },
  watch: {
    radiosender: {
      handler(newSender) {
        console.log(`Aufruf der API mit dem neuen Radiosender: ${newSender}`);
      },
      immediate: true,
    },
  },
};
</script>

<style scoped>
.main {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(115, 115, 226);
}
</style>
