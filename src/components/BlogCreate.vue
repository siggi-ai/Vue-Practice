<template>
  <div>
    <form v-on:submit.prevent="sendPostData">
      <label class="label" for="title">
        <span>Title</span>
      </label>
      <input type="text" id="title" v-model="form.title" placeholder="Title" />
      <label class="label" for="body">
        <span>Artikel</span>
      </label>
      <input type="text" id="body" v-model="form.body" placeholder="Artikel" />
      <label class="label" for="userId">
        <span>Nr</span>
      </label>
      <input
        type="text"
        id="userId"
        v-model.number="form.userId"
        placeholder="Nr"
      />
      <button>Daten speichern</button>
    </form>
  </div>
</template>
<script>
import axios from "axios";
export default {
  name: "BlogCreate",
  data() {
    return {
      form: {
        title: "",
        body: "",
        userId: 0,
      },
    };
  },
  methods: {
    sendPostData() {
      axios
        .post("https://jsonplaceholder.typicode.com/posts", this.form)
        .then((response) => console.log("response:", response))
        .catch((error) => console.log("error: ", error));
    },
  },
};
</script>