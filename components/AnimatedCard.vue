<template>

<div class="container">

    <div class="employee">

     <div class="game">

      <div class="front">
        <div class="front-background">
          <img class="profil" src="../grid-bilder/R1.jpeg" alt="employee">
          <h4 class="name">Philip</h4>
          <div class="stats">
            <p class="viewers">text</p>
            <div class="streamers">
                <img class="bilder" src="../grid-bilder/R2.jpeg" alt="team">
            </div>
          </div>
        </div>
      </div>
        
      <div class="back"></div>
        <div class="streaming-info">
            <p class="game-stat">25.8k<span>Streams</span></p>
            <p class="game-stat">25.8k<span>Streams</span></p>
        </div>
        <button class="btn">Alle Infos zur Person</button>
        <div class="streamer">
          <div class="streamer">
            <p class="name">Info a</p>
            <p class="number">1</p>
          </div>
          <div class="streamer">
            <p class="name">Info b</p>
            <p class="number">2</p>
          </div>
          <div class="streamer">
            <p class="name">Info c</p>
            <p class="number">3</p>
          </div>
        </div>

        <div class="background"></div>
     </div>

    </div>   
</div>

</template>

<script>
export default {};
</script>

<style scoped>

*,
*::before,
*::after {
    box-sizing: border-box;
}

:root {
    --clr-dark: rgb(13, 17, 19);
    --clr-light: #fff;
    --clr-accent: rgb(222, 52, 0);
    --clr-accent-dark: rgb(163, 38, 0);
    --clr-secondary: rgb(0, 62, 163);  

}

.container { 
    font-family: sans-serif;
    min-height: 100vH;
    display: grid;
    place-items: center;
    background: var(--clr-dark);
    color: grey;
}

h1,
h2,
h3,
p {
  margin: 0;
}

img {
  max-width: 100%;
}

.game {
  position: diplay;
  width: 12.5em;
}

.game:hover {  
  transform: scale(1);
}
 

/*
.streamers {
  display: flex;
  width: 2em;
  height: 2em;
  border-radius: 50%;
  
} */
.profil {
  border-radius: 5em;
}

.bilder {
  display: flex;
  width: 2em;
  height: 2em;
  border-radius: 50%;
  align-items: center;
}


.name {
  border: 1px solid grey;
  text-align: center;
  margin: .15em 0;
  border-radius: 5em;
  margin-left: .2em;
  margin-right: .2em
}

.h4 {
  color: grey;
}

.stats {
    display: flex;
    /*justify-content: space-between 0.25em; */
    border: 1px solid red;
    align-items: center;
    border-radius: 5em; 
  }

.streamers img {
  border: 1px solid grey;
  margin-left: 4em;
  z-index: 1;
  
}

.back {
  display: none;
}

.background {
  background: rgb(72, 70, 70);
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: -1;
  opacity: 1;
  border-radius: 5em;
  transform: scale(.4, .7);
}

.front-background:hover {
  transform: translateY(-50%);
}

</style>