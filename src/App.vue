<template>
  <div class="main">
    <h1>Slot Props</h1>
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
