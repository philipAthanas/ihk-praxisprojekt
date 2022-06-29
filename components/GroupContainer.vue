<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div v-if="nav === 'Home'">
      <div class="headIcon" v-if="headIcon">
        <img :src="require('../grid-bilder/Ellipse 1.png')" fluid alt="Icon" />
      </div>
      <div class="employee">
        <div v-for="item in people" v-bind:key="item.name">
          <!-- loop für alle Elemente in people-->
          <!-- item = frei wählbare Variable um die Keys anzusprechen die gerade im Array geloopt werden -->
          <h3>{{ item.name }}</h3>
          <div class="flexbox">
            <img
              class="star"
              :src="require('../grid-bilder/Star 2.png')"
              fluid
              alt="png mit Stern"
              v-if="item.position.length <= 3"
            />
            <h5>{{ item.position }}</h5>
          </div>
        </div>
      </div>
    </div>
    <div
      class="card_Content"
      :data-aos="renderWithFadeIns ? 'flip-down' : ''"
      v-else
    >
      <div class="card_sub_content">
        <img
          :src="require('../grid-bilder/Ellipse 1.png')"
          fluid
          alt="Icon"
          class="head_icon_child"
        />
        <div>
          <h3 class="NameMitarbeiter">{{ people[0].name }}</h3>
          <div class="flexbox_2">
            <img
              class="star"
              :src="require('../grid-bilder/Star 2.png')"
              fluid
              alt="png mit Stern"
              v-if="people[0].position.length <= 3"
            />
            <h5>{{ people[0].position }}</h5>
          </div>
          <br />
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing del, eiusmod
            tempo incididunt ut labore et dolore magna.
          </div>
          <br />
          <div class="employeeContact">
            <p>{{ people[0].tel }}</p>
            <p>{{ people[0].mail }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader", "headIcon", "nav", "renderWithFadeIns"],
};
</script>

<style scoped></style>
