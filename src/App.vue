<template>
  <div class="main">
    <h4>Event Handling</h4>
    <h1>{{ count }}</h1>
    <div>
      <button v-on:click="changeCount(1)">Plus 1</button>
      <button v-on:click="changeCount(5)">Plus 5</button>
      <button v-on:click="changeCount(-1)">Minus 1</button>
      <button v-on:click="changeCount(-5)">Minus 5</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    changeCount(value) {
      this.count = this.count + value;
    },
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
