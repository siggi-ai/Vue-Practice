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
import { reactive, toRefs } from "vue";
export default {
  name: "VModelAPIReactive",
  setup() {
    const state = reactive({
      firstName: "",
      lastName: "",
    });
    return {
      ...toRefs(state),
    };
  },
};
</script>
