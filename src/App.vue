<template>
  <div class="main">
    <h1>Conditional Rendering</h1>
    <div v-if="inzidenzWert > 165" style="background-color: red; color: white">
      Die Inzidenz liegt über 165!
    </div>
    <div v-if="inzidenzWert > 100" style="background-color: red; color: white">
      Die Inzidenz liegt unter 165!
    </div>
    <div v-if="inzidenzWert > 50" style="background-color: red; color: white">
      Die Inzidenz liegt über 50, aber unter 100!
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      inzidenzWert: 75,
    };
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
