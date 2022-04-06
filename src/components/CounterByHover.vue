<template>
  <div>
    <h2 v-on:mouseover="addCount">{{ count }}-mal mit der Maus überfahren</h2>
  </div>
</template>
<script>
export default {
  name: "Counter",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    addCount() {
      this.count += 1;
    },
  },
};
</script>
