<template>
  <div class="content">
    <label class="label" for="firstName">
      <span class="label-text">Vorname</span>
    </label>
    <input 
      type="text"
      id="firstName"
      v-model="firstName"
      placeholder="Vorname"
      class="input"
    >
  </div>
</template>
<script>
export default {
  name: "TabC",
  data () {
    return {
      firstName: "",
    }
  }
};
</script>
<style>
.content {
  padding: 40px;
  font-size: 1.5rem;
}
</style>