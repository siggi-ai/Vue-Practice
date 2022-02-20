<template>
  <div>
    <div>
    <h2>Spielbericht</h2>
    <h3>{{ homeTeam }} gegen {{ guestTeam }}</h3>
    <h4>Zuschauer: {{ spectators }}</h4>
    </div>
    <div>
    <h2>Wurde dieser Spielbericht veröffentlicht?</h2>
    <h3>{{ isPublished ? "Ja" : "Nein" }}</h3>
    </div>
  </div>
</template>
<script>
export default {
    name: "Spielbericht",
    props: {
        homeTeam: {
            type: String,
            required: true,
        },
        guestTeam: {
            type: String,
            required: true
        },
        
    };
};
</script>