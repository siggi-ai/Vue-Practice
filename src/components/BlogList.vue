<template>
  <div>
    <div>
      <button v-on:click="getBlogs">Lade Vorschlag</button>
    </div>
      <div>
        {{ blogs.activity }}
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
  created() {
    this.getBlogs();
  },
  methods: {
    getBlogs() {
      axios
        .get("https://www.boredapi.com/api/activity")
        .then((response) => {
          console.log("response: ", response.data);
          this.blogs = response.data;
        })
        .catch((error) => {
          console.log("error; ", error);
        });
    },
  },
};
</script>