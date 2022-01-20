<template>
  <div class="main">
    <h4>Event Handling</h4>
    <h1>{{ count }}</h1>
    <div>
      <button>Plus</button>
      <button>Plus</button>
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
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
