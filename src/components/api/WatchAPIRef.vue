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
    const firstName = ref("");
    const lastName = ref("");

    watch(
      [firstName, lastName],
      (newValue, oldValue) => {
        console.log("WatchAPIRef firstName old value: ", oldValue[0]);
        console.log("WatchAPIRef firstName new value: ", newValue[0]);
        console.log("WatchAPIRef lastName old value: ", oldValue[1]);
        console.log("WatchAPIRef lastName new value: ", newValue[1]);
      },
      {
        immediate: true,
      }
    );
    return {
      firstName,
      lastName,
    };
  },
};
</script>
