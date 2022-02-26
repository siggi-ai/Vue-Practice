<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ body }}</div>
    <div v-if="actionOn">
      <a v-bind:href="memberLink" target="_blank">Mitglied werden</a>
      <a v-bind:href="webLink" target="_blank">zur website</a>
    </div>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: {
    title: {
      type: String,
    },
    body: {
      type: String,
    },
    actionOn: {
      type: Boolean,
      default: false,
    },
    memberLink: {
      type: String,
    },
    webLink: {
      type: String,
    },
  },
};
</script>
<style>
a {
  padding: 10px;
}
</style>