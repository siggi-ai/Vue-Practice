<template>
  <div class="main">
    <div>
      <h1>Prop Types and Validations</h1>
      <Hallo v-bind:first-name="userName" />
    </div>

    <Spielbericht
      home-team="FC Schalke 04"
      guest-team="Borussia Dortmund"
      v-bind:spectators="70000"
      v-bind:is-published="true"
    />

    <div class="pic"><img src="face.jpg" alt="face" width="100" /></div>
  </div>
</template>

<script>
import Willkommen from "./components/Willkommen.vue";
import Spielbericht from "./components/Spielbericht.vue";
export default {
  name: "App",
  components: {
    Hallo: Willkommen,
    Spielbericht,
  },
  data() {
    return {
      userName: "Hannes",
    };
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
