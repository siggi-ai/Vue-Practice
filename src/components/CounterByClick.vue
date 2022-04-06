<template>
  <div>
    <button v-on:click="addCount">{{ count }}-mal mit der Maus geklickt</button>
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