<template>
  <div class="main">
    <h1>Slots</h1>
    <CardSlot title="HSV" body="Fußballverein">
      <a class="card" href="https://www.hsv.de/uebersicht" target="_blank"
        >Mitglied werden</a
      >
      <a class="card" href="https://www.hsv.de/uebersicht" target="_blank"
        >zur website</a
      >
    </CardSlot>
    <CardSlot title="St Pauli" body="Fußballverein">
      <a class="card" href="https://www.fcstpauli.com/en/" target="_blank"
        >Mitglied werden</a
      >
      <a class="card" href="https://www.fcstpauli.com/en/" target="_blank"
        >zur website</a
      >
    </CardSlot>
  </div>
</template>

<script>
import CardSlot from "./components/CardSlot.vue";
export default {
  name: "App",
  components: {
    CardSlot,
  },
};
</script>

<style>
.card {
  padding: 10px;
  border: 1px solid white;
}
body {
  background-color: rgb(115, 115, 226);
  display: flex;
  text-align: center;
}

.main {
  padding: 100px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(150 150 240);
}

.pic {
  display: flex;
  float: right;
}
</style>
