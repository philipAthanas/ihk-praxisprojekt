<template>
  <div class="square-border">
    <div class="circle" :style="{ backgroundColor: colorCircle }"></div>
    <h4>{{ teamName }}</h4>
  </div>
</template>

<script>
export default {
  props: ["teamName", "colorCircle"],
};
</script>

<style scoped></style>
