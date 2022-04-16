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
    <label for="lastName">
      <span>Nachname</span>
    </label>
    <input
      type="text"
      id="lastName"
      v-model="lastName"
      placeholder="Nachname"
    />
  </div>
</template>
<script>
import { ref } from "vue";
export default {
  name: "VModelAPIRef",
  setup() {
    const firstName = ref("");
    const lastName = ref("");
    return {
      firstName,
      lastName,
    };
  },
};
</script>
