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
import { ref, watch } from "vue";
export default {
  name: "WatchAPIRef",
  //
  setup() {
      const firstName = ref("Klaus");
      const lastName = ref("Fischer");

  watch(firstName, (newValue, oldValue) => {
      console.log("Watch old value: ", oldValue);
      console.log("Watch new value: ", newValue);
    },
    lastName(newValue, oldValue) {
      console.log("Watch old value: ", oldValue);
      console.log("Watch new value: ", newValue);
    }),
  },
};
</script>
