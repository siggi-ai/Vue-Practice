<template>
  <div>
    <div class="main">
      <button v-on:click="showChild = !showChild">Toggle Child</button>
    </div>
    <div class="blogCreate main">
      <Child v-if="showChild" />
    </div>
  </div>
</template>

<script>
import Child from "./Child.vue";

export default {
  name: "Parent",
  data() {
    return {
      showChild: true,
    };
  },
  components: {
    Child,
  },
  beforeCreate() {
    console.log("Parent beforeCreated");
  },
  created() {
    console.log("Parent created");
  },
  beforeMount() {
    console.log("Parent beforeMount");
  },
  mounted() {
    console.log("Parent mounted");
  },
  beforeUpdate() {
    console.log("Parent beforeUpdate");
  },
  updated() {
    console.log("Parent updated");
  },
  beforeUnmount() {
    console.log("Parent beforeUnmount");
  },
  unmounted() {
    console.log("Parent unmounted");
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
  font-size: 1rem;
  margin: 0 auto;
  width: 500px;
  font-family: "Courier New", Courier, monospace;
}
.blogCreate {
  width: 240px;
  text-align: center;
}
</style>