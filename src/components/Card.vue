<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ body }}</div>
    <div>
      <a>Mitglied werden</a>
      <a>zur website</a>
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
  },
};
</script>