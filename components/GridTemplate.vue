<template>
   <body>
    <div class="flex-container" >
      <div class="flex-item">Col 1</div>  
      <div class="flex-item">Col 2</div>
      <div class="flex-item">Col 3</div> 
      <div class="flex-item">Col 4</div>
      <div class="flex-item">Col 5</div>
      <div class="flex-item-team" >
        <div>
        <b-img src="https://picsum.photos/1024/400/?image=41" fluid alt="Responsive image"></b-img>
        </div>
      </div> 
      <div class="flex-item">Col 7</div> 
      <div class="flex-item">Col 8</div>
      <div class="flex-item">Col 9</div>
      <div class="flex-item">Col 10</div> 
      <div class="flex-item">Col 11</div> 
      <div class="flex-item">Col 12</div>
      <div class="flex-item">Col 13</div>
      <div class="flex-item">Col 14</div> 
      <div class="flex-item">Col 15</div> 
      <div class="flex-item">Col 16</div>
      <div class="flex-item">Col 17</div>          
    </div>
    </body>
</template>

<script>
export default {};
</script>

<style scoped>

    body {
        background-color: black;
        color: white;
        font-size: 1rem;
        margin: 0;
    }
    .flex-container {
        display: grid;
        width: 100vw;
        height: 100vh;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-template-rows: auto auto auto auto;
        gap: 10px;
    }
    .flex-item {
        padding: 16px;
        background-color: rgb(0, 157, 255);
        color: white;
        text-align: center;
    }
    .flex-item-team {
        padding: 16px;
        background-color: rgba(0, 157, 255, 0.427);
        grid-column: 2 / span 2;
        grid-row: 2 / span 2;
        justify-self: center;
        align-self: center;
        color: yellow;  
    }
</style>
