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
      <input type="text" v-model="senderInfo.web" />
    </div>
    <div>
      <span>gegründet am:</span>
      <input type="text" v-model="senderInfo.foundedOn" />
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      radiosender: "Delta Radio",
      senderInfo: {
        web: "https://www1.wdr.de/radio/1live/index.html",
        foundedOn: 1998,
      },
    };
  },
  watch: {
    radiosender: {
      handler(newSender) {
        console.log(`Aufruf der API mit dem neuen Radiosender: ${newSender}`);
      },
      immediate: true,
    },
    senderInfo: {
      handler(newInfos) {
        console.log(
          `Aufruf der API mit web "${newInfos.web}" und gegründet am "${newInfos.foundedOn}`
        );
      },
      deep: true,
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
