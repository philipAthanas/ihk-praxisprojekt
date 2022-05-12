<template>

<div class="container-fluid">
    
    <div class="gallery-container">
      <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">1</div>
      </div>
    </div>

    <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">2</div>
      </div>
    </div>

    <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">3</div>
      </div>
    </div>

    <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">4</div>
      </div> 
    </div>

    <div class="gallery-container">
       <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">5</div>
      </div>

    <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">6</div>
      </div>
    </div>

    <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">7</div>
      </div>
    </div>

      <div class="gallery-container">
        <div class="gallery-item">
         <div class="image">
          <img src="https://images.unsplash.com/photo-1558981359-219d6364c9c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80" alt="biker"> <!-- der Link stellt ein random pic zur Verfügung -->    
         </div>
           <div class="text">8</div>
        </div> 
      </div>
 </div>
</div>
</template>

<script>
export default {}
</script>

<style scoped>

.container {
    margin-top: 2rem;
    text-align: center;

    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: 300px 300px;
    grid-gap: 10px;
}

.h1 {
    margin-top: 4rem;
}

.gallery-item {
    width: 100%;
    height: 100%;
    position: relative;
}

.gallery-item .image {
    width: 100%;
    height: 100%;
    overflow: hidden;
}

.gallery-item .image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 50% 50%;
}
</style>