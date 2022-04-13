<template>
  <div>
    <h2>{{ framework }}</h2>
  </div>
</template>
<script>
export default {
  name: "ReactivityAPIA",
  setup() {
    let framework = "Vue 2";
    setTimeout(() => {
      framework = "vue 3";
      console.log("new framework:", framework);
    }, 2000);
    return {
      framework,
    };
  },
};
</script>
