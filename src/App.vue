<template>
  <div class="main">
    <h1>Slots</h1>
    <Card
      title="Schalke 04"
      body="Fußballverein"
      :action-on="true"
      member-link="https://schalke04.de/"
      web-link="https://schalke04.de/"
    />
    <Card
      title="BVB 09"
      body="Fußballverein"
      :action-on="true"
      member-link="https://www.bvb.de/"
      web-link="https://www.bvb.de/"
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
