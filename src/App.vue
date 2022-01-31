<template>
  <div class="main">
    <h2>Eingabebereich</h2>
    <form action="">
      <div>
        <h1>Form Handling</h1>
        <label class="label" for="firstName">
          <span class="label-text">Vorname</span>
        </label>
        <br />
        <input
          type="text"
          id="firstname"
          v-model="form.firstName"
          placeholder="Vorname"
          class="input input-bordered"
        />
        <div>
          <br />
          <label class="label" for="lastName">
            <span class="label-text">Nachname</span>
          </label>
          <br />
          <input
            type="text"
            id="lastname"
            v-model="form.lastName"
            placeholder="Nachname"
            class="input input-bordered"
          />
        </div>
        <div>
          <br />
          <label class="label" for="hobbies">
            <span class="label-text">Hobbys</span>
          </label>
          <br />
          <textarea
            id="hobbies"
            v-model="form.hobbies"
            placeholder="Deine Hobbys"
            class="input input-bordered"
          />
        </div>
        <div>
          <br />
          <label class="label" for="color">
            <span class="label-text">Lieblingsfarbe</span>
          </label>
          <br />
          <select
            id="color"
            class="select select-bordered w-full"
            v-model="form.color"
          >
            <option value="">Wähle Deine Lieblingsfarbe</option>
            <option value="blue">blau</option>
            <option value="red">rot</option>
            <option value="green">grün</option>
          </select>
        </div>
        <div>
          <br />
          <label class="label" for="favoriteArtists">
            <span class="label-text">Lieblingskünstler</span>
          </label>
          <br />
          <select
            id="color"
            class="select select-bordered w-full"
            v-model="form.favoriteArtists"
            multiple
          >
            <option value="">Wähle Deine Lieblingskünstler</option>
            <option value="Kahlo">Kahlo</option>
            <option value="Picasso">Picasso</option>
            <option value="Chagall">Chagall</option>
          </select>
        </div>
        <div>
          <br />
          <label class="label" for="favoriteArtists">
            <input
              type="checkbox"
              id="picture"
              v-model="form.pictureOfTheMonth"
              true-value="ja"
              false-value="nein"
              class="checkbox"
            />
            <span class="label-text"
              >Hast Du schonmal das Bild des Monats produziert?</span
            >
            <br />
          </label>
        </div>
      </div>
    </form>
    <h2>Ausgabebereich</h2>
    <div>
      <div v-for="(item, key, index) in form" :key="index">
        {{ key }}: {{ item }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      form: {
        firstName: "Kai",
        lastName: "Tischler",
        hobbies: "Fußball, Tor des Monats",
        color: "blue",
        favoriteArtists: ["Pablo Picasso"],
        pictureOfTheMonth: false,
      },
    };
  },
};
</script>

<style scoped>
.main {
  padding: 10px;
  font-family: Georgia, "Times New Roman", Times, serif;
}

input {
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
