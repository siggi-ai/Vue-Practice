<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ body }}</div>
    <br />
    <div>
      <slot></slot>
    </div>
    <br />
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