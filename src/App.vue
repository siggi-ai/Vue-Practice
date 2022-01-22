<template>
  <div class="main">
    <h4>Event Handling</h4>
    <h1>{{ name }}</h1>
    <h1>{{ count }}</h1>
    <div>
      <button v-on:click="changeName($event), changeCount(1, $event)">Plus 1</button>
      <button v-on:click="changeCount(5, $event)">Plus 5</button>
      <button v-on:click="changeCount(10, $event)">Plus 10</button>
      <button v-on:click="changeCount(-1, $event)">Minus 1</button>
      <button v-on:click="changeCount(-5, $event)">Minus 5</button>
      <button v-on:click="changeCount(-10, $event)">Minus -10</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: 0,
      name: "Hanni",
    };
  },
  methods: {
    changeCount(value, event) {
      console.log("event: ", event)
      this.count = this.count + value;
    },
    changeName(event) {
      console.log("changeName: ", event);
      this.name = "Bernd";
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
