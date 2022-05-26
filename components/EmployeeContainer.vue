<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div class="employeeDetail">
      <div v-for="item in people" v-bind:key="item.name">
        <div class="headIconDetail" v-if="headIcon">
          <img
            :src="require('../grid-bilder/Ellipse 1.png')"
            fluid
            alt="Icon"
          />
          <h3 class="employeeName">{{ item.name }}</h3>
        </div>

        <img
          class="star"
          :src="require('../grid-bilder/Star 2.png')"
          fluid
          alt="png mit Stern"
        />
        <h5 class="employeeDescription">
          Lorem ipsum dolor sit amet, consectetur adipiscing del, eiusmod tempor
          incididunt ut labore et dolore magna.
        </h5>
        <h5 class="employeePosition">{{ item.position }}</h5>
        <h5>{{ item.tel }}</h5>
        <h5>{{ item.mail }}</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader", "headIcon", "tel", "mail", "nav"],
};
</script>

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
            tel: "MOBIL: + 49 177 8237238",
            mail: "MAIL: b.jawadi@integr8.com",
          },
        ],
        DevelopementTeam: [
          {
            name: "TARIK E.",
            position: "Fullstack Developer",
            tel: "MOBIL: + 49 1573 7532227",
            mail: "MAIL: t.ermis@integr8.com",
          },
          {
            name: "JAKOB S.",
            position: "Fullstack Developer",
            tel: "MOBIL: + 49 000 0000000",
            mail: "MAIL: j.sawal@integr8.com",
          },
          {
            name: "MARVIN K.",
            position: "Web Developer",
            tel: "MOBIL: + 49 175 8300179",
            mail: "MAIL: m.kaddatz@integr8.com",
          },
          {
            name: "LEANDER G.",
            position: "Werkstudent",
            tel: "MOBIL: + 49 176 45880980",
            mail: "MAIL: l.gebhardt@integr8.com",
          },
          {
            name: "PHILIP A.",
            position: "Praktikant",
            tel: "MOBIL: + 49 17684400475",
            mail: "MAIL: p.athanas@integr8.com",
          },
        ],
      },
      teamStrategy: {
        CSO: [
          {
            name: "FLORIS H.",
            position: "CSO",
            tel: "MOBIL: +49 176 818923098",
            mail: "MAIL: f.henning@integr8.com",
          },
        ],
        Director: [
          {
            name: "BLANCA R.",
            position: "Strategy Director",
            tel: "MOBIL: + 49 0162 2409081",
            mail: "MAIL: b.deramonrius@integr8.com",
          },
        ],
        StrategyTeam: [
          {
            name: "DENIS H.",
            position: "Sr. Digital Strategist",
            tel: "MOBIL: + 49 176 844 00 475",
            mail: "MAIL: d.hennes@integr8.com",
          },
          {
            name: "SILJA M.",
            position: "Jr. Strategy",
            tel: "MOBIL: + 49 179 2125261",
            mail: "MAIL: s.marquart@integr8.com",
          },
        ],
      },
      teamCreative: {
        LeadCreative: [
          {
            name: "MARKUS H.",
            position: "Creative Director",
            tel: "MOBIL: + 49 171 8322964",
            mail: "MAIL: m.haupt@integr8.com",
          },
        ],
        CreativeTeam: [
          {
            name: "VIKTOR T.",
            position: "Motion Designer",
            tel: "MOBIL: + 49 17623508534",
            mail: "MAIL: v.tittel@integr8.com",
          },
          {
            name: "ATAHAN Ö.",
            position: "Visual Designer",
            tel: "MOBIL: + 49 000 0000000",
            mail: "MAIL: a.oezbanazi@integr8.com",
          },
          {
            name: "DIVYA K.",
            position: "Brand and Visual Designer",
            tel: "MOBIL: + 49 15170824036",
            mail: "MAIL: d.kowshik@integr8.com",
          },
          {
            name: "HANNA B.",
            position: "Visual Designer",
            tel: "MOBIL: + 49 172 4630611",
            mail: "MAIL: h.biarozka@integr8.com",
          },
          {
            name: "KATHRIN M.",
            position: "Graphic Designer",
            tel: "MOBIL: + 49 176 61240925",
            mail: "MAIL: k.vanmeegen@integr8.com",
          },
          {
            name: "AILEEN D.",
            position: "Praktikantin",
            tel: "MOBIL: + 49 157 34903736",
            mail: "MAIL: s.dorn@integr8.com",
          },
        ],
      },
      teamContent: {
        LeadContent: [
          {
            name: "HANNA S.",
            position: "Head of Content",
            tel: "MOBIL: + 49 176 61049408",
            mail: "MAIL: h.scherber@integr8.com",
          },
        ],
        ContentTeam: [
          {
            name: " MELANIE K.",
            position: "Copywriter",
            tel: "MOBIL: + 49 17680660936",
            mail: "MAIL: m.krause@integr8.com",
          },
        ],
      },
      teamOperation: {
        COO: [
          {
            name: "SUSANNE A.",
            position: "COO",
            tel: "MOBIL: 0049 171 3180860",
            mail: "MAIL: s.anspach@integr8.com",
          },
        ],
        OperationTeam: [
          {
            name: "SARAH K.",
            position: "Sr. Account Manager",
            tel: "MOBIL: 0049 170 4818532",
            mail: "MAIL: s.kollmann@integr8.com",
          },
          {
            name: "JANINA F.",
            position: "Fibu/Lohn BH, Personalberaterin",
            tel: "MOBIL: 0049 176 97807902",
            mail: "MAIL: j.protz@integr8.com",
          },
          {
            name: "RITA V.",
            position: "Culture Managerin",
            tel: "MOBIL: + 49 176 41166622",
            mail: "MAIL: r.valiukonyte@integr8.com",
          },
        ],
      },
      teamMarketing: {
        CMO: [
          {
            name: "MICHAEL R.",
            position: "CMO",
            tel: "MOBIL: 0049 177 8219701",
            mail: "MAIL: m.rutkowski@integr8.com",
          },
        ],
        MarketingTeam: [
          {
            name: "FLORIAN P.",
            position: "Data Analyst",
            tel: "MOBIL: 0049 1578 8881337",
            mail: " MAIL: f.petereit@integr8.com",
          },
          {
            name: "KRYSTYNA G.",
            position: "SEO Managerin",
            tel: "MOBIL: 0049 1575 0967761",
            mail: "MAIL: k.grat@integr8.com",
          },
          {
            name: "ROBERT P.",
            position: "Community Manager",
            tel: "MOBIL: 0049 176 20342084",
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

<style scoped>
.employeeDetail {
  display: flex;
}

.TeamColor {
  width: 100%;
  height: 10px;
  align-self: flex-start;
}

.headIconDetail {
  order: 1;
}

.employeeName {
  order: 2;
}

.employeePosition {
  order: 3;
}

.employeeDescription {
  order: 4;

  font-family: "ProximaNova-Bold";
  color: rgba(0, 0, 0, 1);
  font-size: 16px;
  letter-spacing: 1%;
  align-items: center;
}
</style>
