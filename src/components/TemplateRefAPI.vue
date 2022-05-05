<template>
  <div>
    <label for="firstName" class="label">
      <span>Vorname</span>
    </label>
    <input
      type="text"
      id="firstName"
      ref="refFirstName"
      v-model="firstName"
      placeholder="Vorname"
    />
  </div>
</template>
<script>
import { onMounted, ref } from "vue";
export default {
  name: "TemplateRefAPI",
  //
  setup() {
    const firstName = ref("Gerd");
    const refFirstName = ref(null);
    //
    onMounted(() => {
      refFirstName.value.focus();
    });
    //
    return {
      refFirstName,
      firstName,
    };
  },
};
</script>
