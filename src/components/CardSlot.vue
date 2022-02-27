<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ body }}</div>
    <div>
      <slot></slot>
    </div>
  </div>
</template>
<script>
export default {
  name: "CardSlot",
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
<style>
a {
  padding: 10px;
}
</style>