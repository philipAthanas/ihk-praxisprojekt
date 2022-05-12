<template>

<div class="container">
 

<div class="grid">

    <div class="element item1">1</div>  
    <div class="element item2">2</div>
    <div class="element item3">3</div>
    <div class="element item4">4</div>
    <div class="element item5">5</div>  
    <div class="element item6">6</div>
    <div class="element item7">7</div>
    <div class="element item8">8</div>
    <div class="element item9">9</div>
    <div class="element item10">10</div>
    <div class="element item11">11</div>
    <div class="element item12">12</div>

    <div class="element item13">13</div>  
    <div class="element item14">14</div>
    <div class="element item15">15</div>
    <div class="element item16">16</div>
    <div class="element item17">17</div>  
    <div class="element item18">18</div>
    <div class="element item19">19</div>
    <div class="element item20">20</div>
    <div class="element item21">21</div>
    <div class="element item22">22</div>
    <div class="element item23">23</div>
    <div class="element item24">24</div>

</div>

</div> 

</template>

<script>
export default {
}
</script>

<style scoped>


.container {
  display: grid;
  margin-top: 4rem;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(150px, 100%), 1fr));
  grid-template-rows: repeat(4, 1fr);
  gap: 10px;
  row-gap: 10px;
}
/*
.grid {
  grid-template-rows:    minmax(100px, auto);
  grid-template-columns: minmax(auto, 50%) 1fr 3em;
}
*/

.element {
  border: 1px solid rgb(0, 95, 107);
  border-radius: 3px;
  background-color: rgba(0, 95, 107, 0.8);
  padding: 02.em;
  color: #fff;
  font-size: 1.3rem;
}


.item1 {
  color: black;
  background-color: rgba(66, 224, 245, 0.8);
  grid-column-start: 1;
  grid-column-end: 4;
  grid-row: 1 / 4;
  width: 100%;
  height: 100%;
  align-content: stretch;

}
/*
.item22 {
  color: black;
  background-color: rgba(66, 224, 245, 0.8);
  grid-column-start: 1;
  grid-column-end: 5;
  width: 100%;
  height: 100%;
}


.item24 {
  color: black;
  background-color: rgba(66, 224, 245, 0.8);
  grid-column-start: 2;
  grid-column-end: 4;
  width: 100%;
  height: 100%;
}
*/
</style>