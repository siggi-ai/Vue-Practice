<template>
  <div class="main">
    <div>
      <h1>Custom Component Events</h1>
    </div>
    <button v-on:click="isVisible = true">Popup öffnen</button>
    <Popup v-show="isVisible" v-on:close="closePopup" />
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
      isVisible: false,
    };
  },
  methods: {
    closePopup(name) {
      this.isVisible = false;
      console.log("name is: ", name);
    },
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
