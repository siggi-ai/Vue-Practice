<template>
  <div>
    <h2>Spielbericht</h2>
    <h3>{{ homeTeam }} gegen {{ guestTeam }}</h3>
  </div>
</template>
<script>
export default {
    name: "Spielbericht",
    props: {
        homeTeam {
            type: String,
            required: true,
        },
        guestTeam {
            type: String,
            required: true
        },
    };
}
</script>