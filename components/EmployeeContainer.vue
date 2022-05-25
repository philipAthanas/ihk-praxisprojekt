<template>
  <div>
    <div
      class="TeamColorDetail"
      :style="{ backgroundColor: colorHeader }"
    ></div>
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
  props: ["people", "colorHeader", "headIcon", "tel", "mail"],
};
</script>

<style scoped>
.employeeDetail {
  padding: 5px 5px 5px 5px;
  display: flex;
}

.TeamColorDetail {
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
