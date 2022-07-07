<template>
  <div>
    <div class="header">
      <div
        class="box box1"
        :data-aos="this.renderWithFadeIns ? 'fade-right' : ''"
        data-aos-duration="1000"
      >
        <span class="titel">WIR SIND INTEGR8.</span><br />
        <span class="i8-text"
          ><p>
            <br />
            Als Architekt für den digitalen Raum planen, organisieren und lenken
            wir außergewöhnliche Projekte. Wir entwickeln individuelle Lösungen,
            die Technologie, Kreation und Aktivierung zielführend vereinen. Um
            unser Ziel zu erreichen, bieten wir außergewöhnlichen Talenten eine
            Umgebung, in der sie neues lernen wollen und inspiriert arbeiten
            können.
          </p>
        </span>
      </div>
      <div
        class="box box2_trennlinie"
        :data-aos="this.renderWithFadeIns ? 'zoom-in-up' : ''"
        data-aos-easing="ease-in-back"
        data-aos-delay="400"
        data-aos-offset="-100"
      >
        <img
          class="trenlinie"
          :src="require('../grid-bilder/Line-11.png')"
          fluid
          alt="png mit Trennlinie"
        />
      </div>
      <div
        btn
        class="box box3_dev"
        @click="goto('Developement')"
        :data-aos="this.renderWithFadeIns ? 'flip-down' : ''"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Developement'" :colorCircle="'#00EEBB'" />
      </div>
      <div
        btn
        class="box box4_strategy"
        @click="goto('Operation')"
        :data-aos="this.renderWithFadeIns ? 'flip-down' : ''"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Operation'" :colorCircle="'#FF0000'" />
      </div>
      <div
        btn
        class="box box5_creative"
        @click="goto('Creative')"
        :data-aos="this.renderWithFadeIns ? 'flip-down' : ''"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Creative'" :colorCircle="'#FF7A00'" />
      </div>
      <div
        btn
        class="box box6_operation"
        @click="goto('Strategy')"
        :data-aos="this.renderWithFadeIns ? 'flip-down' : ''"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Strategy'" :colorCircle="'#BD00FF'" />
      </div>
      <div
        btn
        class="box box7_marketing"
        @click="goto('Marketing')"
        :data-aos="this.renderWithFadeIns ? 'flip-down' : ''"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Marketing'" :colorCircle="'#0075FF'" />
      </div>
      <div
        class="box box8_logo"
        @click="nav = 'Home'"
        :data-aos="this.renderWithFadeIns ? 'fade-left' : ''"
        data-aos-duration="1000"
      >
        <img
          class="i8-logo"
          :src="require('../grid-bilder/i8-logo.png')"
          fluid
          alt="INTEGER8 Logo"
        />
      </div>
    </div>
    <div ref="div1"></div>
    <BodyComponent
      :nav="this.nav"
      :selectedMember="this.selectedMember"
      @teamClickedFromBodyComponent="teamClicked"
    />
  </div>
</template>

<script>
export default {
  css: ["~/assets/css/style.css"],
  data() {
    return {
      nav: "Home",
      renderWithFadeIns: true,
      selectedMember: null,
    };
  },
  created() {
    if (window.innerWidth <= 760) {
      console.log("Disable FadeIns");
      this.renderWithFadeIns = false;
    }
  },
  methods: {
    goto(setNav) {
      this.nav = setNav;
      var element = this.$refs["div1"];
      var top = element.offsetTop;
      window.scrollTo(0, top);
    },
    teamClicked(team) {
      // console.log(team);
      this.nav = team[0];
      this.selectedMember = team[1];
    },
  },
};
</script>

<style scoped></style>
