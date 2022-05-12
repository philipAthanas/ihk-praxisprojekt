<template>
<div>
  <div class="Hero container">
   <div class="sticky-top">
     <nav class="navbar navbar-expand-lg navbar-light bg-light">
       <div class="container-fluid">
         <a class="navbar-brand" href="https://www.integr8.com/">I N T E G R 8</a>
          <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
              <li class="nav-item">
                 <a class="nav-link" href="#">i8Plattform</a>
              </li>
            </ul>
          </div>
             <form class="container-fluid">
                <div class="input-group">
                 <span class="input-group-text" id="basic-addon1">@</span>
                   <input type="text" class="form-control" placeholder="Name oder Team suchen" aria-label="Username" aria-describedby="basic-addon1">
                </div>
              </form>
        </div>
     </nav>
    </div> 
    <b-row>
      <b-col>
        <div class="text-container">
          <div data-aos="zoom-in" >
          <h2 class="header">INTEGR8</h2>
          <h4 class="subtitle">Organigramm</h4>
          <p class="snippet">Alle Teams und alle Mitarbeitenden der INTEGR8 media GmbH auf einen Blick. Wählbar in der Übersicht als Funktionseinheit oder in der personalisierten Detailansicht.</p>
         </div>
        </div>
      </b-col>
      <b-col>
        <div data-aos="zoom-in-up" data-aos-delay="1200">
        <img src="data:image/png;base64,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" class="image" alt="i8">
      </div>
      </b-col>
    </b-row>
    <b-form-select v-model="selected" :options="options" size="m" class="mt-3"/>
    <div class="mt-3">Selected: Du hast das Team <strong>{{ selected }}</strong> ausgewählt</div>
  </div>
  <!--<img src="https://www.integr8.com/wp-content/uploads/2021/11/integr8_preview.png"> class="image" alt="i8">-->


  <div class="grid">
   <div class="row r1">
      <div class="col-12 col-lg-6" 
      style="border:1px solid red;">
      1
            <div class="card">
        <div class="card-content">
          <h4 class="card-title">Philip Athanas</h4> 
          <h5 class="card-body">Praktikant</h5>
          <a href="#" class="button">Details</a>
        </div>
    </div>
      </div>

      <div class="col-12 col-lg-6" 
      style="border:1px solid red;">
      2
          <div class="row">
      <div class="col-12 col-lg-3 col-md-8" 
      style="border:1px solid red;">
      3
            <div class="card">
        <div class="card-content">
          <h4 class="card-title">Philip Athanas</h4> 
          <h5 class="card-body">Praktikant</h5>
          <a href="#" class="button">Details</a>
        </div>
    </div>
      </div>

      <div class="col-12 col-lg-3 col-md-8" 
      style="border:1px solid red;">
      4
            <div class="card">
        <div class="card-content">
          <h4 class="card-title">Philip Athanas</h4> 
          <h5 class="card-body">Praktikant</h5>
          <a href="#" class="button">Details</a>
        </div>
    </div>
      </div>
        <div class="col-12 col-lg-3 col-md-8" 
      style="border:1px solid red;">
      5
            <div class="card">
        <div class="card-content">
          <h4 class="card-title">Philip Athanas</h4> 
          <h5 class="card-body">Praktikant</h5>
          <a href="#" class="button">Details</a>
        </div>
    </div>
      </div>

      <div class="col-12 col-lg-3 col-md-8" 
      style="border:1px solid red;">
      6
            <div class="card">
        <div class="card-content">
          <h4 class="card-title">Philip Athanas</h4> 
          <h5 class="card-body">Praktikant</h5>
          <a href="#" class="button">Details</a>
        </div>
    </div>
      </div>
      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      3
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      4
      </div>
        <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      5
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      6
      
      </div>
   </div>
      </div>
    </div>
  </div>

<section class="section-1"> 
    <div class="row r1">
      <div class="col-12 col-lg-6 e1" 
      style="border:1px solid red;">
      1
      </div>

      <div class="col-12 col-lg-6" 
      style="border:1px solid red;">
      2
          <div class="row">
      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      3
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      4
      </div>
        <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      5
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      6
      
      </div>
      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      3
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      4
      </div>
        <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      5
      </div>

      <div class="col-12 col-lg-3 col-md-4" 
      style="border:1px solid red;">
      6
      
      </div>
   </div>
      </div>
    </div>
  </section> 


<div>
    <b-row>
      <b-col>
          <div data-aos="fade-up" data-aos-delay="300">
            <img class="img-logo" img src="data:image/png;base64,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">
         </div>     
      </b-col>
    </b-row>
  </div>


</div> 
</template>

<script>
export default {
  data () {
    return {
      selected: null,
      options: [
        { value: 'Team auswählen', text: 'Team auswählen' },
        { value: 'Accounting/Controlling', text: 'Accounting/Controlling' },
        { value: 'Business Developement', text: 'Business Developement' },
        { value: 'Creative', text: 'Creative' },
        { value: 'Developement', text: 'Developement' },
        { value: 'Human Resources', text: 'Human Resources' },
        { value: 'Management', text: 'Management' },
        { value: 'Office Management', text: 'Office Management' },
        { value: 'Performance', text: 'Performance' },
        { value: 'Social Media', text: 'Social Media' },
        { value: 'Strategy', text: 'Strategy' }
      ]
    }
  },
   css: [
    '~/assets/css/main.css'
  ]
}
</script>
