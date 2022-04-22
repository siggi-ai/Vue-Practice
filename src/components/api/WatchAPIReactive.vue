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
    <input
      type="text"
      id="offensiveAPIReaction"
      v-model.number="skills.offensive"
      placeholder="Offensivfähigkeit"
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
      skills: {
        offensive: 9,
      },
    });
    watch(
      () => state.firstName,
      function (newValue, oldValue) {
        console.log("WatchAPIReactive old value: ", oldValue);
        console.log("WatchAPIReactive new value: ", newValue);
      }
    );
    return {
      ...toRefs(state),
    };
  },
};
</script>
