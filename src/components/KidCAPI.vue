<template>
  <div>
    <h4>Kid C</h4>
    <p>Spieler: {{ firstName }} {{ lastName }}</p>
    <p>erzielte Bundesligatore: {{ childGoals }}</p>
  </div>
</template>
<script>
import { inject, toRefs } from "vue";
export default {
  name: "KidCAPI",
  //
  setup() {
    const childGoals = inject("c_goals", 0);
    const childPlayer = inject("c_player", {
      firstName: "Klaus",
      lastName: "Fischer",
    });
    //
    return {
      childGoals,
      ...toRefs(childPlayer),
    };
  },
};
</script>
