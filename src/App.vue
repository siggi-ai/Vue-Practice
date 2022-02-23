<template>
  <div class="main">
    <div>
      <h1>Custom Component Events</h1>
    </div>

    <button
      v-on:click="isInvisible = !isInvisible"
      v-on:close="isVisible = false"
    >
      <p>
        öffnen <br />
        schließen
      </p>
    </button>
    <br />
    <br />
    <button onclick="alert('Thank you!')">be polite</button>
    <Popup v-show="isInvisible" />
  </div>
</template>

<script>
import Popup from "./components/Popup.vue";
export default {
  name: "App",
  components: {
    Popup,
  },
  data() {
    return {
      isInvisible: false,
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
