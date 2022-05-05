<template>
  <div>
    <h3>ProvideInjectAPI</h3>
    <p>Spieler {{ firstName }} {{ lastName }}</p>
    <p>erzielte Bundesligatore: {{ goals }}</p>
    <KidA />
  </div>
</template>
<script>
import { provide, ref, reactive, toRefs } from "vue";
import KidA from "./KidAAPI.vue";
export default {
  name: "ProvideInjectAPI",
  //
  components: {
    KidA,
  },
  setup() {
    const goals = ref(329);
    const state = reactive({
      firstName: "Gerd",
      lastName: "Müller",
    });
    //
    provide("c_goals", goals);
    provide("c_player", state);
    //
    return {
      goals,
      ...toRefs(state),
    };
  },
};
</script>
