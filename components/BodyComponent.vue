<template>
  <div>
    <div class="body nav_home" v-if="nav === 'Home'">
      <div class="team1" data-aos="zoom-in-right" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamDev.CTO"
          :colorHeader="'#00eebb'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team8" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamDev.DevelopementTeam"
          :colorHeader="'#00eebb'"
          :nav="nav"
        />
      </div>
      <div class="team2" data-aos="zoom-in" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamStrategy.CSO"
          :colorHeader="'#BD00FF'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team5" data-aos="zoom-in" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamStrategy.Director"
          :colorHeader="'#BD00FF'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team9" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamStrategy.StrategyTeam"
          :colorHeader="'#BD00FF'"
          :nav="nav"
        />
      </div>
      <div class="team6" data-aos="zoom-in" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamCreative.LeadCreative"
          :colorHeader="'#FF7A00'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team10" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamCreative.CreativeTeam"
          :colorHeader="'#FF7A00'"
          :nav="nav"
        />
      </div>
      <div class="team7" data-aos="zoom-in" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamContent.LeadContent"
          :colorHeader="'#FF7A00'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team11" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamContent.ContentTeam"
          :colorHeader="'#FF7A00'"
          :nav="nav"
        />
      </div>
      <div class="team3" data-aos="zoom-in" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamOperation.COO"
          :colorHeader="'#FF0000'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team12" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamOperation.OperationTeam"
          :colorHeader="'#FF0000'"
          :nav="nav"
        />
      </div>
      <div class="team4" data-aos="zoom-in-left" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamMarketing.CMO"
          :colorHeader="'#0075FF'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
      <div class="team13" data-aos="fade-up" data-aos-duration="1500">
        <GroupContainer
          :people="this.teamMarketing.MarketingTeam"
          :colorHeader="'#0075FF'"
          :nav="nav"
        />
      </div>
      <div class="line1" data-aos="zoom-in" data-aos-duration="1500">
        <img :src="require('../grid-bilder/Line 1.png')" fluid alt="Linie 1" />
      </div>
      <div class="lineNew1" data-aos="zoom-in" data-aos-duration="1500"></div>
      <div class="line2" data-aos="zoom-in" data-aos-duration="1500">
        <img :src="require('../grid-bilder/Line 2.png')" fluid alt="Linie 2" />
      </div>
      <div class="line3" data-aos="zoom-in" data-aos-duration="1500">
        <img :src="require('../grid-bilder/Line 3.png')" fluid alt="Linie 3" />
      </div>
      <div class="line4" data-aos="zoom-in" data-aos-duration="1500">
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
      <div class="group36" data-aos="zoom-in" data-aos-duration="1500">
        <img
          :src="require('../grid-bilder/Group 36.png')"
          fluid
          alt="Group 36"
        />
      </div>

      <div class="line8" data-aos="zoom-in" data-aos-duration="1500">
        <img :src="require('../grid-bilder/Line 8.png')" fluid alt="Linie 8" />
      </div>
      <div class="line9" data-aos="zoom-in" data-aos-duration="1500">
        <img :src="require('../grid-bilder/Line 9.png')" fluid alt="Linie 9" />
      </div>
      <div class="line10" data-aos="zoom-in" data-aos-duration="1500">
        <img
          :src="require('../grid-bilder/Line 10.png')"
          fluid
          alt="Linie 10"
        />
      </div>
    </div>

    <div class="unit" v-if="nav === 'Developement'">
      <div
        class="card_Parent"
        v-for="teamMember in [
          ...this.teamDev.CTO,
          ...this.teamDev.DevelopementTeam,
        ]"
        v-bind:key="teamMember.name"
      >
        <GroupContainer
          :people="[teamMember]"
          :colorHeader="'#00eebb'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
    </div>
    <div class="unit" v-if="nav === 'Strategy'">
      <div
        class="card_Parent"
        v-for="teamMember in [
          ...this.teamStrategy.CSO,
          ...this.teamStrategy.Director,
          ...this.teamStrategy.StrategyTeam,
        ]"
        v-bind:key="teamMember.name"
      >
        <GroupContainer
          :people="[teamMember]"
          :colorHeader="'#BD00FF'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
    </div>
    <div class="unit" v-if="nav === 'Creative'">
      <div
        class="card_Parent"
        v-for="teamMember in [
          ...this.teamCreative.LeadCreative,
          ...this.teamCreative.CreativeTeam,
          ...this.teamContent.LeadContent,
          ...this.teamContent.ContentTeam,
        ]"
        v-bind:key="teamMember.name"
      >
        <GroupContainer
          :people="[teamMember]"
          :colorHeader="'#FF7A00'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
    </div>
    <div class="unit" v-if="nav === 'Operation'">
      <div
        class="card_Parent"
        v-for="teamMember in [
          ...this.teamOperation.COO,
          ...this.teamOperation.OperationTeam,
        ]"
        v-bind:key="teamMember.name"
      >
        <GroupContainer
          :people="[teamMember]"
          :colorHeader="'#FF0000'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
    </div>
    <div class="unit" v-if="nav === 'Marketing'">
      <div
        class="card_Parent"
        v-for="teamMember in [
          ...this.teamMarketing.CMO,
          ...this.teamMarketing.MarketingTeam,
        ]"
        v-bind:key="teamMember.name"
      >
        <GroupContainer
          :people="[teamMember]"
          :colorHeader="'#0075FF'"
          :headIcon="true"
          :nav="nav"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["nav"],
  css: ["~/assets/css/style.css"],
  data() {
    return {
      title: "Name",
      teamDev: {
        CTO: [
          {
            name: "BAHAR J.",
            position: "CTO",
            tel: "MOBIL: 0177 8237238",
            mail: "MAIL: b.jawadi@integr8.com",
          },
        ],
        DevelopementTeam: [
          {
            name: "TARIK E.",
            position: "Fullstack Developer",
            tel: "MOBIL: 01573 7532227",
            mail: "MAIL: t.ermis@integr8.com",
          },
          {
            name: "JAKOB S.",
            position: "Fullstack Developer",
            tel: "MOBIL: 0170 0000000",
            mail: "MAIL: j.sawal@integr8.com",
          },
          {
            name: "MARVIN K.",
            position: "Web Developer",
            tel: "MOBIL: 0175 8300179",
            mail: "MAIL: m.kaddatz@integr8.com",
          },
          {
            name: "LEANDER G.",
            position: "Werkstudent",
            tel: "MOBIL: 0176 45880980",
            mail: "MAIL: l.gebhardt@integr8.com",
          },
          {
            name: "PHILIP A.",
            position: "Praktikant",
            tel: "MOBIL: 0176 84400475",
            mail: "MAIL: p.athanas@integr8.com",
          },
        ],
      },
      teamStrategy: {
        CSO: [
          {
            name: "FLORIS H.",
            position: "CSO",
            tel: "MOBIL: 0176 818923098",
            mail: "MAIL: f.henning@integr8.com",
          },
        ],
        Director: [
          {
            name: "BLANCA R.",
            position: "Strategy Director",
            tel: "MOBIL: 0162 2409081",
            mail: "MAIL: b.deramonrius@integr8.com",
          },
        ],
        StrategyTeam: [
          {
            name: "DENIS H.",
            position: "Sr. Digital Strategist",
            tel: "MOBIL: 0170 00000000",
            mail: "MAIL: d.hennes@integr8.com",
          },
          {
            name: "SILJA M.",
            position: "Jr. Strategy",
            tel: "MOBIL: 0179 2125261",
            mail: "MAIL: s.marquart@integr8.com",
          },
        ],
      },
      teamCreative: {
        LeadCreative: [
          {
            name: "MARKUS H.",
            position: "Creative Director",
            tel: "MOBIL: 0171 8322964",
            mail: "MAIL: m.haupt@integr8.com",
          },
        ],
        CreativeTeam: [
          {
            name: "VIKTOR T.",
            position: "Motion Designer",
            tel: "MOBIL: 0176 23508534",
            mail: "MAIL: v.tittel@integr8.com",
          },
          {
            name: "ATAHAN Ö.",
            position: "Visual Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "MAIL: a.oezbanazi@integr8.com",
          },
          {
            name: "DIVYA K.",
            position: "Brand and Visual Designer",
            tel: "MOBIL: 0151 70824036",
            mail: "MAIL: d.kowshik@integr8.com",
          },
          {
            name: "HANNA B.",
            position: "Visual Designer",
            tel: "MOBIL: 0172 4630611",
            mail: "MAIL: h.biarozka@integr8.com",
          },
          {
            name: "KATHRIN M.",
            position: "Graphic Designer",
            tel: "MOBIL: 0176 61240925",
            mail: "MAIL: k.vanmeegen@integr8.com",
          },
          {
            name: "AILEEN D.",
            position: "Praktikantin",
            tel: "MOBIL: 0157 34903736",
            mail: "MAIL: s.dorn@integr8.com",
          },
        ],
      },
      teamContent: {
        LeadContent: [
          {
            name: "HANNA S.",
            position: "Head of Content",
            tel: "MOBIL: 0176 61049408",
            mail: "MAIL: h.scherber@integr8.com",
          },
        ],
        ContentTeam: [
          {
            name: " MELANIE K.",
            position: "Copywriter",
            tel: "MOBIL: 0176 80660936",
            mail: "MAIL: m.krause@integr8.com",
          },
        ],
      },
      teamOperation: {
        COO: [
          {
            name: "SUSANNE A.",
            position: "COO",
            tel: "MOBIL: 0171 3180860",
            mail: "MAIL: s.anspach@integr8.com",
          },
        ],
        OperationTeam: [
          {
            name: "SARAH K.",
            position: "Sr. Account Manager",
            tel: "MOBIL: 0170 4818532",
            mail: "MAIL: s.kollmann@integr8.com",
          },
          {
            name: "JANINA F.",
            position: "Fibu/Lohn BH, Personalberaterin",
            tel: "MOBIL: 0176 97807902",
            mail: "MAIL: j.protz@integr8.com",
          },
          {
            name: "RITA V.",
            position: "Culture Managerin",
            tel: "MOBIL: 0176 41166622",
            mail: "MAIL: r.valiukonyte@integr8.com",
          },
        ],
      },
      teamMarketing: {
        CMO: [
          {
            name: "MICHAEL R.",
            position: "CMO",
            tel: "MOBIL: 0177 8219701",
            mail: "MAIL: m.rutkowski@integr8.com",
          },
        ],
        MarketingTeam: [
          {
            name: "FLORIAN P.",
            position: "Data Analyst",
            tel: "MOBIL: 01578 8881337",
            mail: " MAIL: f.petereit@integr8.com",
          },
          {
            name: "KRYSTYNA G.",
            position: "SEO Managerin",
            tel: "MOBIL: 01575 0967761",
            mail: "MAIL: k.grat@integr8.com",
          },
          {
            name: "ROBERT P.",
            position: "Community Manager",
            tel: "MOBIL: 0176 20342084",
            mail: "MAIL:  r.piotrowicz@integr8.com",
          },
          {
            name: "SERDAR S.",
            position: "Sr. Performance Marketing Manager",
            tel: "MOBIL: 0172 4113348",
            mail: "MAIL: s.saglam@integr8.com",
          },
          {
            name: "TIM F.",
            position: "Marketing Strategist",
            tel: "MOBIL: 0172 5954655",
            mail: "MAIL: t.franzke@integr8.com",
          },
        ],
      },
    };
  },
};
</script>

<style scoped></style>
