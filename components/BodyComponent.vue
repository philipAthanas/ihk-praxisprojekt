<template>
  <div class="body">
    <GroupContainer :people="this.team.CTO" :colorHeader="'green'" />
    <GroupContainer :people="this.team.DevelopementTeam" :colorHeader="'red'" />
  </div>
</template>

<script>
export default {
  css: ["~/assets/css/style.css"],
  data() {
    return {
      title: "Name",
      team: {
        CTO: [{ name: "Bahar J.", position: "CTO" }],
        DevelopementTeam: [
          { name: "Tarik E.", position: "Fullstack Developer" },
          { name: "Jakob S.", position: "Fullstack Developer" },
          { name: "Marvin K.", position: "Web Developer" },
          { name: "Leander G.", position: "Web Developer" },
          { name: "Philip A.", position: "Praktikant Development" },
        ],
      },
    };
  },
};
</script>

<style scoped></style>
