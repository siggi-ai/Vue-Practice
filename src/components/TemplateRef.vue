<template>
  <div>
    <label for="firstName" class="label"></label>
    <input
      type="text"
      id="firstName"
      ref="firstName"
      v-model="firstName"
      placeholder="Vorname"
    />
  </div>
</template>
<script>
export default {
  name: "TemplateRef",
  //
  data() {
    return {
      firstName: "Hans",
    };
  },
  //
  mounted() {
    this.$refs.firstName.focus();
  },
};
</script>
