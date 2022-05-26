<template>
  <div>
    <div class="testArea" v-if="nav === 'Home'">
      <div class="testBox 1">
        <div>
          <div class="employeeHeadIcon">
            <img
              :src="require('../grid-bilder/Ellipse 1.png')"
              fluid
              alt="Icon"
            />
            <div v-for="item in people" v-bind:key="item.name">
              <h3>{{ item.name }}</h3>
              <h3 class="employeeName">{{ item.name }}</h3>
            </div>
          </div>
        </div>
        <GroupContainer :people="this.teamDev.CTO" :colorHeader="'#00eebb'" />
        <div h5 class="employeeDescription">
          Lorem ipsum dolor sit amet, consectetur adipiscing del, eiusmod tempor
          incididunt ut labore et dolore magna.
        </div>
        <div h5 class="employeeContakt">
          <span>MOBILE: 0176 0000000</span><br />
          <span>MAIL: b.jawadi@integr8.com</span>
        </div>
      </div>

      <div class="testBox 2">
        <h1>2</h1>
      </div>
      <div class="testBox 3">
        <h1>3</h1>
      </div>
      <div class="testBox 4">
        <h1>4</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader", "headIcon", "nav"],
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
            tel: "MOBIL 0177 8237238",
            mail: "MAIL b.jawadi@integr8.com",
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
.testArea {
  border: solid 2px;
  display: flex;
  width: 100%;
  padding: 5% 5%;

  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
}

.testBox1 {
  display: flex;
  color: black;
  padding: 7% 7%;
}

.employeeDetail {
}

.TeamColor {
  width: 100%;
  height: 10px;
  position: relative;
  top: -5rem;
}

.employeeHeadIcon {
  position: relative;
  top: 6rem;
}

.employeeName {
  justify-content: left;
  right: 6rem;
}

.employeePosition {
}

.employeeDescription {
  font-family: "ProximaNova-Bold";
  color: rgba(0, 0, 0, 1);
  font-size: 16px;
  letter-spacing: 1%;
}

.employeeContakt {
  font-family: "ProximaNova-Bold";
  padding: 10px;
}

.star {
}
</style>
