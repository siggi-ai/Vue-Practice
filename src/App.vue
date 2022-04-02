<template>
  <div class="main">
    <h1>Teleport</h1>
    <teleport to="#portal">
      <Portal />
    </teleport>
  </div>
</template>

<script>
import Portal from "./components/Portal";

export default {
  name: "App",
  components: {
    Portal,
  },
};
</script>

<style scoped>
body {
  background-color: rgb(115, 115, 226);
}
.main {
  text-align: center;
  margin-left: 0 auto;
  padding: 30px;
  font-size: 2rem;
  margin: 0 auto;
  width: 500px;
  font-family: 'Courier New', Courier, monospace;
}
</style>
