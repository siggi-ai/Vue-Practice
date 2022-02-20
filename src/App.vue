<template>
  <div class="main">
    <div>
      <h1>first child</h1>
      <Hallo v-bind:first-name="userName" />
    </div>

    <div class="pic"><img src="face.jpg" alt="face" width="100"/></div>
  </div>
</template>

<script>
import Willkommen from "./components/Willkommen.vue";
export default {
  name: "App",
  components: {
    Hallo: Willkommen,
  },
  data () {
    return {
      userName: "Hannes",
    }
  }
};
</script>

<style>
body {
  background-color: rgb(115, 115, 226);
  display: flex;
}

.main {
  padding: 100px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(150 150 240);
}


</style>
