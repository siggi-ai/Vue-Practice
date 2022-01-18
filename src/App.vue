<template>
  <div class="main">
    <h4>
      Multipliziere die Variable price mit dem normalen Mehrwertsteuersatz
    </h4>
    <div>
      Steuersatz: {{ taxRate }}
      <br />
      Netto-Preis: {{ price2 }}
      <br />
      Brutto-Preis: {{ multiply(price2) }}
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      price1: 100,
      price2: 200,
      taxRate: 19,
    };
  },
  methods: {
    multiply(num) {
      return (num * (100 + this.taxRate)) / 100;
    },
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
