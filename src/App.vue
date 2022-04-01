<template>
  <div>
    <div class="main">
      <h1>Dynamic Component</h1>
      <button
        v-on:click="tabActive = 'TabA'"
        class="tab"
        v-bind:class="{ 'tab-active': tabActive === 'TabA' }"
      >
        A
      </button>
      <button
        v-on:click="tabActive = 'TabB'"
        class="tab"
        v-bind:class="{ 'tab-active': tabActive === 'TabB' }"
      >
        B
      </button>
      <button
        v-on:click="tabActive = 'TabC'"
        class="tab"
        v-bind:class="{ 'tab-active': tabActive === 'TabC' }"
      >
        C
      </button>
    </div>
    <div>
      <TabA v-if="tabActive === 'TabA'" />
      <TabB v-if="tabActive === 'TabB'" />
      <TabC v-if="tabActive === 'TabC'" />
    </div>
  </div>
</template>

<script>
import TabA from "./components/TabA.vue";
import TabB from "./components/TabB.vue";
import TabC from "./components/TabC.vue";
export default {
  name: "App",
  components: {
    TabA,
    TabB,
    TabC,
  },
  data() {
    return {
      tabActive: "TabA",
    };
  },
};
</script>

<style scoped>
body {
  background-color: rgb(115, 115, 226);
  text-align: center;
}
.main {
  margin-left: 0 auto;
}
h4 {
  color: orange;
  font-size: 1.4rem;
}
</style>
