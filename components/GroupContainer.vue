<template>
  <div>
    <div class="TeamColor" :style="{ backgroundColor: colorHeader }"></div>
    <div v-for="item in people" v-bind:key="item.name">
      <!-- item = frei wählbare Variable um die Keys anzusprechen die gerade im Array geloopt werden -->
      <h1>{{ item.name }}</h1>
      <h1>{{ item.position }}</h1>
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
