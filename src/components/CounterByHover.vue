<template>
  <div>
    <h2 v-on:mouseover="addCount">{{ count }}-mal mit der Maus überfahren</h2>
  </div>
</template>
<script>
import CounterMixin from "../mixins/counter";
export default {
  name: "Counter",
  data() {
    return {
      counter: 100,
    };
  },
  mixins: [CounterMixin],
  
};
</script>
