<template>
  <div class="main">
    <h1>Watchers</h1>
    <h2>Lautstärke</h2>
    <h3>
      <progress v-bind:value="volume" max="5"></progress>
    </h3>
    <h4>{{ volume }}</h4>
    <button v-on:click="volume -= 1">-</button>
    <button v-on:click="volume += 1">+</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      volume: 0,
    };
  },
  watch: {
    
  }
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
