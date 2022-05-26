<template>
  <div>
    <div class="header">
      <div class="box box1" data-aos="fade-right" data-aos-duration="1000">
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
        data-aos="zoom-in-up"
        data-aos-easing="ease-in-back"
        data-aos-delay="400"
        data-aos-offset="-100"
      >
        <img
          class="trenlinie"
          :src="require('../grid-bilder/Line 11.png')"
          fluid
          alt="png mit Trennlinie"
        />
      </div>
      <div
        btn
        class="box box3_dev"
        @click="nav = 'Developement'"
        data-aos="flip-down"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Developement'" :colorCircle="'#00EEBB'" />
      </div>
      <div
        btn
        class="box box4_strategy"
        @click="nav = 'Operation'"
        data-aos="flip-down"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Operation'" :colorCircle="'#FF0000'" />
      </div>
      <div
        btn
        class="box box5_creative"
        @click="nav = 'Creative'"
        data-aos="flip-down"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Creative'" :colorCircle="'#FF7A00'" />
      </div>
      <div
        btn
        class="box box6_operation"
        @click="nav = 'Strategy'"
        data-aos="flip-down"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Strategy'" :colorCircle="'#BD00FF'" />
      </div>
      <div
        btn
        class="box box7_marketing"
        @click="nav = 'Marketing'"
        data-aos="flip-down"
        data-aos-duration="1000"
      >
        <TeamBox :teamName="'Marketing'" :colorCircle="'#0075FF'" />
      </div>

      <div
        class="box box8_logo"
        @click="nav = 'Home'"
        data-aos="fade-left"
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
    <BodyComponent :nav="this.nav" />
    <!-- nach dem : Variable in Anführungszeichen der Value -->
    <TestComponent :nav="this.nav" />
  </div>
</template>

<script>
export default {
  css: ["~/assets/css/style.css"],

  data() {
    return {
      nav: "Home",
    };
  },
};
</script>

<style scoped></style>
