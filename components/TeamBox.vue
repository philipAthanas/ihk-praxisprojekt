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

<style scoped>
.circle {

  
  width: 20px;
  height: 20px;
  border-radius: 100%;
}

.square-border {
  
  display: flex;
  background: #FFF;
  border: 1px solid #000000;
  padding: 22px;
  text-align: center;
  align-items: center;
  
}

h4 {
  margin: 0px;
  margin-left: 15px;
}
</style>