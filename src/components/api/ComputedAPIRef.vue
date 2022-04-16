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
    <h2>Hello {{ fullName }} !</h2>
  </div>
</template>
<script>
import { ref, computed } from "vue";
export default {
  name: "ComputedAPIRef",
  setup() {
    const firstName = ref("");
    const lastName = ref("");
    //
    const fullName = computed(function () {
      return `${firstName.value} ${lastName.value}`;
    });
    //
    return {
      firstName,
      lastName,
      fullName,
    };
  },
};
</script>