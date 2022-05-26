<template>
  <div class="testArea" v-if="nav === 'Home'">
    <div class="testBox1">
      <h1>1</h1>
    </div>
    <div class="testBox2">
      <h1>2</h1>
    </div>
    <div class="testBox3">
      <h1>3</h1>
    </div>
    <div class="testBox4">
      <h1>4</h1>
    </div>
  </div>
</template>

<script>
export default { props: ["colorHeader", "nav"] };
</script>

<style scoped></style>
