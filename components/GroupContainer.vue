<template>
  <div>
    <div>
      <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
      <div v-if="nav === 'Home'">
        <div class="headIcon" v-if="headIcon">
          <img
            :src="require('../grid-bilder/Ellipse 1.png')"
            fluid
            alt="Icon"
          />
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
      <div class="testBox 2" data-aos="flip-down" v-else>
        <div class="employeeHeadIcon_2">
          <img
            :src="require('../grid-bilder/Ellipse 1.png')"
            fluid
            alt="Icon"
          />
          <div class="content">
            <div h3 class="NameMitarbeiter">{{ people[0].name }}</div>
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
            <div>
              Lorem ipsum dolor sit amet, consectetur adipiscing del, eiusmod
              tempo incididunt ut labore et dolore magna.
            </div>
            <div>
              <h5>{{ people[0].tel }}</h5>
              <span>{{ people[0].mail }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader", "headIcon", "nav"],
};
</script>

<style scoped>
.employee {
  padding: 50px 50px 0px 50px;
}

.TeamColor {
  width: 100%;
  height: 10px;
  align-self: flex-start;
}

.flexbox {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-family: "ProximaNova-Bold";
  margin-bottom: 50px;
}

.headIcon {
  position: absolute;
  top: -32px;
  left: 0;
  right: 0;
  z-index: 1;
}
</style>
