<template>
  <div class="main">
    <h1>Slot Props</h1>
    <div>
      <PlayersList>
        <template v-slot:default="slotProps">
          {{ slotProps.firstName }} 
          {{ slotProps.lastName }}
          <br />
          Alter: {{ slotProps.age }}
        </template>
      </PlayersList>
    </div>
  </div>
</template>

<script>
import PlayersList from "./components/PlayersList.vue";
export default {
  name: "App",
  components: {
    PlayersList,
  },
};
</script>

<style>
.card {
  padding: 10px;
  border: 1px solid white;
}
body {
  background-color: rgb(115, 115, 226);
  display: flex;
  text-align: center;
}

.main {
  padding: 100px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(150 150 240);
}

.pic {
  display: flex;
  float: right;
}
</style>
