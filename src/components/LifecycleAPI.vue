<template>
  <div>
    <h5>Lifecycle Hooks in LifecycleAPI</h5>
  </div>
</template>
<script>
import {
  onBeforeMount,
  onMounted,
  onBeforeUpdate,
  onUpdated,
  onBeforeUnmount,
  onUnmounted,
} from "vue";
export default {
  name: "LifecycleAPI",
  //
  setup() {
    console.log("LifecycleAPI created");
    onBeforeMount(() => {
      console.log("LifecycleAPI onBeforeMount");
    });
    onMounted(() => {
      console.log("LifecycleAPI onMounted");
    });
    onBeforeUpdate(() => {
      console.log("LifecycleAPI onBeforeUpdate");
    });
    onUpdated(() => {
      console.log("LifecycleAPI onUpdated");
    });
    onBeforeUnmount(() => {
      console.log("LifecycleAPI onBeforeUnmount");
    });
    onUnmounted(() => {
      console.log("LifecycleAPI onUnmounted");
    });
  },
};
</script>
