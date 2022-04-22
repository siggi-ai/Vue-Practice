<template>
  <div>
    <label for="firstName">
      <span>Vorname</span>
    </label>
    <input
      type="text"
      id="firstName"
      v-model="firstName"
      placeholder="Vorname"
    />
    <input
      type="text"
      id="lastName"
      v-model="lastName"
      placeholder="Nachname"
    />
  </div>
</template>
<script>
import { reactive, toRefs, watch } from "vue";
export default {
  name: "WatchAPIReactive",
  //
  setup() {
    const state = reactive({
      firstName: "Uwe",
      lastName: "Seeler",
    });
    watch(
      state,
      function (newValue, oldValue) {
        console.log("WatchAPIReactive old value: ", oldValue);
        console.log("WatchAPIReactive new value: ", newValue);
      },
      {
        immediate: true,
      }
    );
    return {
      ...toRefs(state),
    };
  },
};
</script>
