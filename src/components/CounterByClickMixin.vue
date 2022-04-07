<template>
  <div>
    <button v-on:click="addCount" class="button">
      {{ count }}-mal mit der Maus geklickt
    </button>
  </div>
</template>
<script>
import CounterMixin from "../mixins/counter";
export default {
  name: "CounterByClickMixin",
  mixins: [CounterMixin],
  methods: {
    addCount() {
      this.count += 1;
    },
  },
};
</script>
<style>
.button {
  background-color: aqua;
  width: 120px;
  height: 100px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-size: 20px;
}
</style>