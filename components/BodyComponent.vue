<template>
  <div class="body">
    <div class="team1">
      <GroupContainer :people="this.teamDev.CTO" :colorHeader="'green'" />
      <GroupContainer
        :people="this.teamDev.DevelopementTeam"
        :colorHeader="'green'"
      />
    </div>
    <div class="team2">
      <GroupContainer :people="this.teamStrategy.CSO" :colorHeader="'pink'" />
      <GroupContainer
        :people="this.teamStrategy.StrategyTeam"
        :colorHeader="'pink'"
      />
    </div>
    <div class="team3">
      <GroupContainer
        :people="this.teamCreative.LeadCreative"
        :colorHeader="'orange'"
      />
    </div>
    <div class="team4">
      <GroupContainer
        :people="this.teamCreative.CreativeTeam"
        :colorHeader="'orange'"
      />
    </div>
    <div class="team5">
      <GroupContainer :people="this.teamOperation.COO" :colorHeader="'red'" />
      <GroupContainer
        :people="this.teamOperation.OperationTeam"
        :colorHeader="'red'"
      />
    </div>
    <div class="team6">
      <GroupContainer :people="this.teamMarketing.CMO" :colorHeader="'blue'" />
      <GroupContainer
        :people="this.teamMarketing.MarketingTeam"
        :colorHeader="'blue'"
      />
    </div>
  </div>
</template>

<script>
export default {
  css: ["~/assets/css/style.css"],
  data() {
    return {
      title: "Name",
      teamDev: {
        CTO: [{ name: "BAHAR J.", position: "CTO" }],
        DevelopementTeam: [
          { name: "TARIK E.", position: "Fullstack Developer" },
          { name: "JAKOB S.", position: "Fullstack Developer" },
          { name: "MARVIN K.", position: "Web Developer" },
          { name: "LEANDER G.", position: "Web Developer" },
          { name: "PHILIP A.", position: "Praktikant" },
        ],
      },
      teamStrategy: {
        CSO: [{ name: "FLORIS H.", position: "CSO" }],
        StrategyTeam: [
          { name: "BLANCA R.", position: "Strategy Director" },
          { name: "DENIS H.", position: "Sr. Digital Strategist" },
          { name: "SILJA M.", position: "Jr. Strategy" },
        ],
      },
      teamCreative: {
        LeadCreative: [{ name: "MARKUS H.", position: "Creative Director" }],
        CreativeTeam: [
          { name: "VIKTOR T.", position: "Motion Designer" },
          { name: "ATAHAN Ö.", position: "Visual Designer" },
          { name: "DIVYA K.", position: "Brand and Visual Designer" },
          { name: "HANNA B.", position: "Visual Designer" },
          { name: "KATHRIN M.", position: "Graphic Designer" },
        ],
      },
      teamOperation: {
        COO: [{ name: "SUSANNE A.", position: "COO" }],
        OperationTeam: [
          { name: "SARAH K.", position: "Sr. Account Manager" },
          { name: "JANINA F.", position: "Fibu/Lohn BH, Personalberaterin" },
          { name: "RITA V.", position: "Culture Managerin" },
        ],
      },
      teamMarketing: {
        CMO: [{ name: "MICHAEL R.", position: "CMO" }],
        MarketingTeam: [
          { name: "FLORIAN P.", position: "Data Analyst" },
          { name: "KRYSTYNA G.", position: "SEO Managerin" },
          { name: "ROBERT P.", position: "Community Manager" },
          { name: "SERDAR S.", position: "Sr. Performance Marketing Manager" },
          { name: "TIM F.", position: "Marketing Strategist" },
        ],
      },
    };
  },
};
</script>

<style scoped></style>
