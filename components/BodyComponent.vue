<template>
  <div
    class="body"
    :class="
      this.nav === 'Home'
        ? 'nav_home'
        : this.nav === 'Strategy'
        ? 'nav_strategy'
        : 'nav_development'
    "
  >
    <div class="team1" @click="nav = 'Strategy'">
      <GroupContainer
        :people="this.teamDev.CTO"
        :colorHeader="'green'"
        :headIcon="true"
      />
    </div>
    <div class="team8">
      <GroupContainer
        :people="this.teamDev.DevelopementTeam"
        :colorHeader="'green'"
      />
    </div>
    <div class="team2">
      <GroupContainer
        :people="this.teamStrategy.CSO"
        :colorHeader="'pink'"
        :headIcon="true"
      />
    </div>
    <div class="team5">
      <GroupContainer
        :people="this.teamStrategy.Director"
        :colorHeader="'pink'"
        :headIcon="true"
      />
    </div>
    <div class="team9">
      <GroupContainer
        :people="this.teamStrategy.StrategyTeam"
        :colorHeader="'pink'"
      />
    </div>
    <div class="team6">
      <GroupContainer
        :people="this.teamCreative.LeadCreative"
        :colorHeader="'orange'"
        :headIcon="true"
      />
    </div>
    <div class="team10">
      <GroupContainer
        :people="this.teamCreative.CreativeTeam"
        :colorHeader="'orange'"
      />
    </div>
    <div class="team7">
      <GroupContainer
        :people="this.teamContent.LeadContent"
        :colorHeader="'orange'"
        :headIcon="true"
      />
    </div>
    <div class="team11">
      <GroupContainer
        :people="this.teamContent.ContentTeam"
        :colorHeader="'orange'"
      />
    </div>
    <div class="team3">
      <GroupContainer
        :people="this.teamOperation.COO"
        :colorHeader="'red'"
        :headIcon="true"
      />
    </div>
    <div class="team12">
      <GroupContainer
        :people="this.teamOperation.OperationTeam"
        :colorHeader="'red'"
      />
    </div>
    <div class="team4">
      <GroupContainer
        :people="this.teamMarketing.CMO"
        :colorHeader="'blue'"
        :headIcon="true"
      />
    </div>
    <div class="team13">
      <GroupContainer
        :people="this.teamMarketing.MarketingTeam"
        :colorHeader="'blue'"
      />
    </div>
    <div class="line1">
      <img :src="require('../grid-bilder/Line 1.png')" fluid alt="Linie 1" />
    </div>
    <div class="line2">
      <img :src="require('../grid-bilder/Line 2.png')" fluid alt="Linie 2" />
    </div>
    <div class="line3">
      <img :src="require('../grid-bilder/Line 3.png')" fluid alt="Linie 3" />
    </div>
    <div class="line4">
      <img :src="require('../grid-bilder/Line 4.png')" fluid alt="Linie 4" />
    </div>
    <!--
    <div class="line5">
      <img :src="require('../grid-bilder/Line 5.png')" fluid alt="Linie 5" />
    </div>
    <div class="line6">
      <img :src="require('../grid-bilder/Line 6.png')" fluid alt="Linie 6" />
    </div>
    -->
    <div class="group36">
      <img :src="require('../grid-bilder/Group 36.png')" fluid alt="Group 36" />
    </div>

    <div class="line8">
      <img :src="require('../grid-bilder/Line 8.png')" fluid alt="Linie 8" />
    </div>
    <div class="line9">
      <img :src="require('../grid-bilder/Line 9.png')" fluid alt="Linie 9" />
    </div>
    <div class="line10">
      <img :src="require('../grid-bilder/Line 10.png')" fluid alt="Linie 10" />
    </div>
    <div class="card1">
      <h1>Card1</h1>
    </div>
    <div class="card2">
      <h1>Card2</h1>
    </div>
    <div class="card3">
      <h1>Card3</h1>
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
        CTO: [
          {
            name: "BAHAR J.",
            position: "CTO",
            tel: "623486123548",
            mail: "bahar@integr8.com",
          },
        ],
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
        Director: [{ name: "BLANCA R.", position: "Strategy Director" }],
        StrategyTeam: [
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
      teamContent: {
        LeadContent: [{ name: "HANNA B.", position: "Visual Designer" }],
        ContentTeam: [{ name: " MELANIE K.", position: "Copywriter" }],
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
      nav: "Home",
    };
  },
};
</script>

<style scoped></style>
