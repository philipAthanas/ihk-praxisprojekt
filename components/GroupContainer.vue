<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div class="headIcon"
    v-if="headIcon" >
      <img :src="require('../grid-bilder/Ellipse 1.png')" fluid alt="Icon" />
       
       </div>
      <div class="employee">
        <div v-for="item in people" v-bind:key="item.name">
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
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader", "headIcon"],
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
