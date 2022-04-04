<template>
  <div>
    <div>
      <label class="label" for="firstName">
        <span>Vorname</span>
      </label>
      <input type="text" ref="firstName" id="firstName" />
    </div>
  </div>
</template>
<script>
export default {
  name: "TemplateRef",
  mounted() {
    this.$refs.firstName.focus();
  },
};
</script>
