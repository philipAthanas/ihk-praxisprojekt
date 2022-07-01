<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div v-if="nav === 'Home'">
      <div class="headIcon" v-if="headIcon">
        <img :src="require('../grid-bilder/Ellipse 1.png')" fluid alt="Icon" />
      </div>
      <div class="employee">
        <div
          v-for="item in people"
          v-bind:key="item.name"
          @click="clickOnTeamMember(item)"
        >
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
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing del, eiusmod
            tempo incididunt ut labore et dolore magna.
          </p>
          <div class="employeeContact">
            <p>{{ people[0].tel }}</p>
            <div class="mail_container">
              <p>MAIL:</p>
              <a :href="`mailto:${people[0].mail}`">
                <p>{{ people[0].mail }}</p>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: [
    "people",
    "colorHeader",
    "headIcon",
    "nav",
    "renderWithFadeIns",
    "team",
    "selectedMember",
  ],
  mounted() {
    // console.log("selectedMember", this.$props);
  },
  methods: {
    clickOnTeamMember(member) {
      this.$emit("teamClicked", [this.$props.team, member.name]);
    },
  },
};
</script>

<style scoped>
.mail_container {
  display: flex;
  flex-direction: row;
}
</style>
