<template>
  <div>
    <div class="header">
      <div class="box box1">
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

      <div class="box box2">
        <img
          class="trenlinie"
          :src="require('../grid-bilder/Line 11.png')"
          fluid
          alt="png mit Trennlinie"
        />
      </div>
      <div class="box box3" @click="nav = 'Developement'">
        <TeamBox :teamName="'Developement'" :colorCircle="'#00EEBB'" />
      </div>
      <div class="box box4" @click="nav = 'Operation'">
        <TeamBox :teamName="'Operation'" :colorCircle="'#FF0000'" />
      </div>
      <div class="box box5" @click="nav = 'Creative'">
        <TeamBox :teamName="'Creative'" :colorCircle="'#FF7A00'" />
      </div>
      <div class="box box6" @click="nav = 'Strategy'">
        <TeamBox :teamName="'Strategy'" :colorCircle="'#BD00FF'" />
      </div>
      <div class="box box7" @click="nav = 'Marketing'">
        <TeamBox :teamName="'Marketing'" :colorCircle="'#0075FF'" />
      </div>

      <div class="box box8" @click="nav = 'Home'">
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
