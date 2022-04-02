<template>
  <div>
    <div>
      <button v-on:click="getBlogs">Lade die Blog-Artikel</button>
    </div>
  </div>
</template>
<script>
import axios from "axios";
export default {
  name: "BlogList",
  data() {
    return {
      blogs: [],
    };
  },
  methods: {
    getBlogs() {
      axios
        .get("https://catfact.ninja/fact")
        .then((response) => {
          console.log("response: ", response.data);
        })
        .catch((error) => {
          console.log("error; ", error);
        });
    },
  },
};
</script>