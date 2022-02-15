<template>
  <div class="main">
    <h1>computed properties</h1>
    <h2>{{ fullName }} {{ title }}</h2>
    <h3>
      There once was a person called
      {{ fullName }}, who was called {{ title }} by everyone. She lived in a
      great {{ home }} and ate a lot of {{ food }}. But in the woods next to her
      {{ home }}, there also lived an evil {{ enemy }}. {{ firstName }} was
      afraid, the {{ enemy }} could attack her. Her cook had an idea. He 
      prepared a {{ powerFood }} and served it to his master.
      <br />
      One day, when the {{ enemy }} approached the {{ home }}, {{ firstName }}
      looked out of the window and became afraid. She immediatly ordered
      {{ powerFood }} and ate it all at once.
    </h3>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: "Clara",
      lastName: "Fall",
      title: "the Greatest",
      home: "castle",
      food: "pizza",
      enemy: "dragon",
    };
  },
  computed: {
    fullName: {
      get() {
        return `${this.firstName} ${this.lastName}`;
      },
      set(value) {
        const names = value.split(" ");
        this.firstName = names[0];
        this.lastName = names[1];
      }
    },
    powerFood() {
      return `${this.enemy}${this.food}`
    }
  },
};
</script>

<style scoped>
.main {
  padding: 50px;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: rgb(115, 115, 226);
}
</style>
