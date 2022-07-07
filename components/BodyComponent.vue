<template>
  <div>
    <div class="body nav_home" v-if="nav === 'Home'">
      <div
        class="team1"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamDev.CTO"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          colorHeader="#00eebb"
          team="Developement"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team8"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamDev.DevelopementTeam"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          colorHeader="#00eebb"
          team="Developement"
          @teamClicked="teamClicked"
          :selectedMember="selectedMember"
        />
      </div>
      <div
        class="team2"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamStrategy.CSO"
          :colorHeader="'#BD00FF'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Strategy"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team5"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamStrategy.Director"
          :colorHeader="'#BD00FF'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Strategy"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team9"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamStrategy.StrategyTeam"
          :colorHeader="'#BD00FF'"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Strategy"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team6"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamCreative.LeadCreative"
          :colorHeader="'#FF7A00'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Creative"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team10"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamCreative.CreativeTeam"
          :colorHeader="'#FF7A00'"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Creative"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team7"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamContent.LeadContent"
          :colorHeader="'#FF7A00'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Content"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team11"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamContent.ContentTeam"
          :colorHeader="'#FF7A00'"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Content"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team3"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamOperation.COO"
          :colorHeader="'#FF0000'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Operation"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team12"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamOperation.OperationTeam"
          :colorHeader="'#FF0000'"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Operation"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team4"
        :data-aos="renderWithFadeIns ? 'zoom-in-left' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamMarketing.CMO"
          :colorHeader="'#0075FF'"
          :headIcon="true"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Marketing"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="team13"
        :data-aos="renderWithFadeIns ? 'fade-up' : ''"
        data-aos-duration="1500"
      >
        <GroupContainer
          :people="this.teamMarketing.MarketingTeam"
          :colorHeader="'#0075FF'"
          :nav="nav"
          :renderWithFadeIns="renderWithFadeIns"
          team="Marketing"
          @teamClicked="teamClicked"
        />
      </div>
      <div
        class="line1"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line2"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line3"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line4"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line5"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line6"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="line7"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="strich"></div>
        <div class="kreise"></div>
      </div>
      <div
        class="gl"
        :data-aos="renderWithFadeIns ? 'zoom-in-right' : ''"
        data-aos-duration="1500"
      >
        <div class="kreise"></div>
        <div class="kreise"></div>
        <div class="kreise"></div>
        <div class="kreise"></div>
        <div class="strich_horizontal"></div>
        <div class="strich_vertical"></div>
        <div class="strich_vertical"></div>
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
          :renderWithFadeIns="renderWithFadeIns"
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
          :renderWithFadeIns="renderWithFadeIns"
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
          :renderWithFadeIns="renderWithFadeIns"
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
          :renderWithFadeIns="renderWithFadeIns"
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
          :renderWithFadeIns="renderWithFadeIns"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["nav", "selectedMember"],
  css: ["~/assets/css/style.css"],
  data() {
    return {
      renderWithFadeIns: true,
      teamDev: {
        CTO: [
          {
            name: "TEAMLEAD",
            position: "CTO",
            tel: "MOBIL: 0170 0000000",
            mail: "developement@integr8.com",
          },
        ],
        DevelopementTeam: [
          {
            name: "EMPLOYEE",
            position: "Fullstack Developer",
            tel: "MOBIL: 0170 0000000",
            mail: "developement@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Web Developer",
            tel: "MOBIL: 0170 0000000",
            mail: "developement@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Werkstudent",
            tel: "MOBIL: 0170 0000000",
            mail: "developement@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Praktikant",
            tel: "MOBIL: 0170 0000000",
            mail: "developement@integr8.com",
          },
        ],
      },
      teamStrategy: {
        CSO: [
          {
            name: "TEAMLEAD",
            position: "CSO",
            tel: "MOBIL: 0170 0000000",
            mail: "strategy@integr8.com",
          },
        ],
        Director: [
          {
            name: "EMPLOYEE",
            position: "Strategy Director",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
        ],
        StrategyTeam: [
          {
            name: "EMPLOYEE",
            position: "Sr. Digital Strategist",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Jr. Strategy",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Werkstudent",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Jr. Strategist",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Digital Product Designer",
            tel: "MOBIL: 0170 00000000",
            mail: "strategy@integr8.com",
          },
        ],
      },
      teamCreative: {
        LeadCreative: [
          {
            name: "TEAMLEAD",
            position: "Creative Director",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
        ],
        CreativeTeam: [
          {
            name: "EMPLOYEE",
            position: "Motion Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Visual Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Brand and Visual Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Visual Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Graphic Designer",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Praktikantin",
            tel: "MOBIL: 0170 0000000",
            mail: "creative@integr8.com",
          },
        ],
      },
      teamContent: {
        LeadContent: [
          {
            name: "TEAMLEAD",
            position: "Head of Content",
            tel: "MOBIL: 0170 0000000",
            mail: "content@integr8.com",
          },
        ],
        ContentTeam: [
          {
            name: "EMPLOYEE",
            position: "Copywriter",
            tel: "MOBIL: 0170 0000000",
            mail: "content@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Copywriter",
            tel: "MOBIL: 0170 0000000",
            mail: "content@integr8.com",
          },
        ],
      },
      teamOperation: {
        COO: [
          {
            name: "TEAMLEAD",
            position: "COO",
            tel: "MOBIL: 0170 0000000",
            mail: "operation@integr8.com",
          },
        ],
        OperationTeam: [
          {
            name: "EMPLOYEE",
            position: "Sr. Account Manager",
            tel: "MOBIL: 0170 0000000",
            mail: "operation@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Fibu/Lohn BH, Personalberaterin",
            tel: "MOBIL: 0170 0000000",
            mail: "operation@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Culture Managerin",
            tel: "MOBIL: 0170 0000000",
            mail: "operation@integr8.com",
          },
        ],
      },
      teamMarketing: {
        CMO: [
          {
            name: "TEAMLEAD",
            position: "CMO",
            tel: "MOBIL: 0170 0000000",
            mail: "marketing@integr8.com",
          },
        ],
        MarketingTeam: [
          {
            name: "EMPLOYEE",
            position: "SEO Managerin",
            tel: "MOBIL: 0170 0000000",
            mail: "marketing@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Community Manager",
            tel: "MOBIL: 0170 0000000",
            mail: "marketing@integr8.com",
          },
          {
            name: "EMPLOYEE",
            position: "Sr. Performance Marketing Manager",
            tel: "MOBIL: 0170 0000000",
            mail: "marketing@integr8.com",
          },
        ],
      },
    };
  },
  created() {
    console.log(this.$props);
    if (window.innerWidth <= 760) {
      console.log("Disable FadeIns");
      this.renderWithFadeIns = false;
    }
  },
  methods: {
    teamClicked(team) {
      this.$emit("teamClickedFromBodyComponent", team);
    },
  },
};
</script>

<style scoped></style>
