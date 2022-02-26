<template>
  <div class="main">
    <h1>Slots</h1>
    <Card
      class="card"
      title="HSV"
      body="Fußballverein"
      :action-on="true"
      member-link="https://www.hsv.de/uebersicht"
      web-link="https://www.hsv.de/uebersicht"
    />
    <Card
      class="card"
      title="FC St. Pauli"
      body="Fußballverein"
      :action-on="true"
      member-link="https://www.fcstpauli.com/"
      web-link="https://www.fcstpauli.com/"
    />
  </div>
</template>

<script>
import Card from "./components/Card.vue";
export default {
  name: "App",
  components: {
    Card,
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
