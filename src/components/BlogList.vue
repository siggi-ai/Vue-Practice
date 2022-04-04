<template>
  <div>
    <!--     <div>
      <button v-on:click="getBlogs">Lade Vorschlag</button>
    </div> -->
    <div v-for="blog in blogs" :key="blog.id">
      <div>
        <h2>{{ blog.title }}</h2>
        {{ blogs.body }}
      </div>
    </div>
  </div>
</template>
<script>
import axios from "axios";
export default {
  name: "BlogList",
  created() {
    this.getBlogs();
  },
  data() {
    return {
      blogs: [],
    };
  },
  methods: {
    getBlogs() {
      axios
        .get("https://jsonplaceholder.typicode.com/posts")
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