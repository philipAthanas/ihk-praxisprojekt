<template>
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

    <div class="box box3">
      <TeamBox :teamName="'Developement'" :colorCircle="'green'" />
    </div>

    <div class="box box4">
      <TeamBox :teamName="'Operation'" :colorCircle="'red'" />
    </div>
    <div class="box box5">
      <TeamBox :teamName="'Creative'" :colorCircle="'orange'" />
    </div>
    <div class="box box6">
      <TeamBox :teamName="'Strategy'" :colorCircle="'purple'" />
    </div>
    <div class="box box7">
      <TeamBox :teamName="'Marketing'" :colorCircle="'blue'" />
    </div>

    <div class="box box8">
      <img
        class="i8-logo"
        :src="require('../grid-bilder/i8-logo.png')"
        fluid
        alt="INTEGER8 Logo"
      />
    </div>
  </div>
</template>

<script>
export default {
  css: ["~/assets/css/style.css"],
};
</script>

<style scoped></style>
