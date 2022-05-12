<template>
 <div class="parent-background">
  <div class="child-background">
   <b-row class="Avatare">
    <b-col>
      <div>
        <div data-aos="flip-left"
        data-aos-easing="ease-out-cubic"
        data-aos-duration="2000">
        <div><strong>Management</strong></div>p>
          <div class="Kreisbilder">
            <b-avatar variant="primary"></b-avatar>
            <b-avatar variant="dark"></b-avatar>
            <b-avatar variant="info"></b-avatar>
          </div>
        </div> 
      </div> 
      <div>
        <div data-aos="fade-right"
        data-aos-offset="300"
        data-aos-easing="ease-in-sine">
        <b-list-group style="max-width: 300px;">
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar class="mr-3"></b-avatar>
            <span class="mr-auto">Team Member 1</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar class="mr-3"></b-avatar>
            <span class="mr-auto">Team Member 2</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar class="mr-3"></b-avatar>
            <span class="mr-auto">Team Member 3</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
        </b-list-group>
        </div>
      </div>
    </b-col>
   </b-row>
  </div>
 </div> 
</template>

<script>
export default {}
</script>

<style scoped>
.parent {
  height: 200px;
  width: 100%;
  background-color: white;
}
.child {
  background-color: red;
  height: 200%;
  width: 100%;
  translate: transform 2s;
}
.parent:hover .child {
         background-color: rgb(0, 0, 0);
         transform:translateX(100%);
}

.Avatare {
    margin-top: 2rem;
    margin-bottom: 2rem;
    margin-left: 40%;
}
.Kreisbilder {
    margin-bottom: 2rem;
    transform: translateX(50%);
}
</style>
