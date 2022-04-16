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
import { reactive, toRefs, computed } from "vue";
export default {
  name: "ComputedAPIReactive",
  setup() {
    const state = reactive({
      firstName: "",
      lastName: "",
    });
    const fullName = computed(function () {
      return `${state.firstName} ${state.lastName}`;
    });
    //
    return {
      ...toRefs(state),  
      fullName,
    };
  },
};
</script>