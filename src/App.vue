<template>
  <div class="main">
    <h4>Event Handling</h4>
    <h1>{{ name }}</h1>
    <div>
      <button v-on:click="name = 'Annalena'">Ändere den Namen</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Angela",
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
