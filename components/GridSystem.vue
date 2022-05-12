<template>

<container class="container">

<section class="basic-grid">
  <div class="card">1</div>
  <div class="card">2</div>
  <div class="card">3</div>
  <div class="card">4</div>
  <div class="card">5</div>
  <div class="card">6</div>
  <div class="card">7</div>
  <div class="card">8</div>
  <div class="card">9</div>
  <div class="card">10</div>
  <div class="card">11</div>
  <div class="card">12</div>
  
</section>

<section>
<h1 class="headline">Photo Gallery Grid</h1>

<div class="photo-grid">

 <div
        class="card card-tall card-wide"
        style="background-image:url('https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80')"
      >
        1
      </div>
      <div
        class="card card-tall"
        style="background-image:url('https://images.unsplash.com/photo-1583585635793-0e1894c169bd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=913&q=80')"
      >
        2
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583531172005-814191b8b6c0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=975&q=80')"
      >
        3
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583426573939-97d09302d76a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=968&q=80')"
      >
        4
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583532452513-a02186582ccd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80')"
      >
        5
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583445013765-46c20c4a6772?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80')"
      >
        6
      </div>
      <div
        class="card card-wide"
        style="background-image:url('https://images.unsplash.com/photo-1583562835057-a62d1beffbf3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=949&q=80')"
      >
        7
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583483425010-c566431a7710?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1951&q=80')"
      >
        8
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583500557349-fb5238f8d946?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1949&q=80')"
      >
        9
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583468323330-9032ad490fed?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1955&q=80')"
      >
        10
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583425423320-2386622cd2e4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1980&q=80')"
      >
        11
      </div>
      <div
        class="card"
        style="background-image:url('https://images.unsplash.com/photo-1583518257225-f9a8081f6a84?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80')"
      >
        12
      </div>
</div>
</section>

<h1 class="headline">Animated Cards</h1>

<section class="animated-grid">
  <div class="card">a</div>
  <div class="card">b</div>
  <div class="card">c</div>
  <div class="card">d</div>
  <div class="card">e</div>
  <div class="card">f</div>
  <div class="card">g</div>
  <div class="card">h</div>
  <div class="card">i</div>
  <div class="card">j</div>
  <div class="card">k</div>
  <div class="card">l</div>
  <div class="card">main</div>
</section>


</container>

</template>

<script>
export default {};
</script>

<style scoped>



.container {
  margin-top: 6rem;
  margin-bottom: 20rem;
}

.headline {
  margin-top: 6rem;
}

.gallery-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px, 300px));
}

body {
    background: rgb(19, 19, 19);
    color: #fff;
    font-family: 'Noto Sans', sans-serif;
}


   
.basic-grid {
    display: grid;
    gap: 1rem;

    /* 1 too skinny, too much code */
    /* grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr; */
  
    /* 2 cleaner code */
    /* grid-template-columns: repeat(12, 1fr); */
  
    /* 3  better sizing, but overflows */
    /* grid-template-columns: repeat(12, minmax(240px, 1fr)); */
  
    /* 4 final */
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
 }

.card {
    display: grid;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: #353535;
    font-size: 3rem;
    color: #fff;
    box-shadow: rgba(3, 8, 20, 0.1) 0px 0.15rem 0.5rem, rgba(2, 8, 20, 0.1) 0px 0.075rem 0.175rem;
    height: 100%;
    width: 100%;
    border-radius: 4px;
    transition: all 500ms;
    overflow: hidden;

    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
 }
  
.card:hover {
    box-shadow: rgba(2, 8, 20, 0.1) 0px 0.35em 1.175em, rgba(2, 8, 20, 0.08) 0px 0.175em 0.5em;
    transform: translateY(-3px) scale(1.1);
 }


 .photo-grid {
  display: grid;
  gap: 1rem;
  margin-top: 6rem;

  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  grid-auto-rows: 240px;
}

/* Medium screens */
@media screen and (min-width: 600px) {
  .card-tall {
    grid-row: span 2 / auto;
  }

  .card-wide {
    grid-column: span 2 / auto;
  }
}

.animated-grid {
  height: 85vh;
  margin-bottom: 200px;

  display: grid;
  gap: 1rem;

  /* Explicit grid */
  grid-template-areas:
    'a  b  c  d'
    'l  🌟 🌟 e'
    'k  🌟 🌟 f'
    'j  i  h  g';

  grid-template-rows: repeat(4, 25%);
  grid-template-columns: 240px auto auto 240px;

  --stagger-delay: 100ms;
}

@keyframes cardEntrance {
  from {
    opacity: 0;
    transform: scale(0.3);
    filter: hue-rotate(180deg);
  }
  to {
    opacity: 1;
    transform: scale(1);
    filter: hue-rotate(0deg);
  }
}

.card-animated {
  margin-top: 6rem;
  background-color: rgb(36, 243, 147);
  animation: cardEntrance 700ms ease-out;
  animation-fill-mode: backwards;
}

.card-animated:nth-child(1) {
  grid-area: a;
  animation-delay: calc(1 * var(--stagger-delay));
}
.card-animated:nth-child(2) {
  grid-area: b;
  animation-delay: calc(2 * var(--stagger-delay));
}
.card-animated:nth-child(3) {
  grid-area: c;
  animation-delay: calc(3 * var(--stagger-delay));
}
.card-animated:nth-child(4) {
  grid-area: d;
  animation-delay: calc(4 * var(--stagger-delay));
}
.card-animated:nth-child(5) {
  grid-area: e;
  animation-delay: calc(5 * var(--stagger-delay));
}
.card-animated:nth-child(6) {
  grid-area: f;
  animation-delay: calc(6 * var(--stagger-delay));
}
.card-animated:nth-child(7) {
  grid-area: g;
  animation-delay: calc(7 * var(--stagger-delay));
}
.card-animated:nth-child(8) {
  grid-area: h;
  animation-delay: calc(8 * var(--stagger-delay));
}
.card-animated:nth-child(9) {
  grid-area: i;
  animation-delay: calc(9 * var(--stagger-delay));
}
.card-animated:nth-child(10) {
  grid-area: j;
  animation-delay: calc(10 * var(--stagger-delay));
}
.card-animated:nth-child(11) {
  grid-area: k;
  animation-delay: calc(11 * var(--stagger-delay));
}
.card-animated:nth-child(12) {
  grid-area: l;
  animation-delay: calc(12 * var(--stagger-delay));
}
.card-animated:last-child {
  grid-area: 🌟;
  animation-delay: calc(13 * var(--stagger-delay));
}




</style>