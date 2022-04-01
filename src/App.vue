<template>
  <div>
    <div class="main">
      <h1>Dynamic Component</h1>
      <button
        v-on:click="tabActivate = 'TabA'"
        class="tab"
        v-bind:class="{ 'tab-activate': tabActive === 'TabA' }"
      >
        A
      </button>
      <button
        v-on:click="tabActivate = 'TabB'"
        class="tab"
        v-bind:class="{ 'tab-activate': tabActive === 'TabB' }"
      >
        B
      </button>
      <button
        v-on:click="tabActivate = 'TabC'"
        class="tab"
        v-bind:class="{ 'tab-activate': tabActive === 'TabC' }"
      >
        C
      </button>
    </div>
    <div>
      <TabA v-if="tabActivate === 'TabA'" />
      <TabB v-if="tabActivate === 'TabB'" />
      <TabC v-if="tabActivate === 'TabC'" />
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
      tabActivate: "TabA",
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
