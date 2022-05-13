<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div v-for="item in people" v-bind:key="item.name">
      <!-- item = frei wählbare Variable um die Keys anzusprechen die gerade im Array geloopt werden -->
      <h3>{{ item.name }}</h3>
      <h5>{{ item.position }}</h5>
    </div>
  </div>
</template>

<script>
export default {
  props: ["people", "colorHeader"],
};
</script>

<style scoped>
.TeamColor {
  width: 100%;
  height: 2px;
}
</style>
