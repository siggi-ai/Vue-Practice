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
      v-model="firstName"
      placeholder="Vorname"
    />
  </div>
</template>
<script>
export default {
  name: "VModelAPIReactive",
};
</script>
