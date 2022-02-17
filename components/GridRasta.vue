<template>
  <b-row class="Avatare">
    <b-col>
      <div>
        <p><strong>Developement Team</strong><p />
        <div class="Kreisbilder">
          <b-avatar variant="info"></b-avatar>
          <b-avatar variant="secondary"></b-avatar>
          <b-avatar variant="primary"></b-avatar>
        </div>
        <b-list-group style="max-width: 300px;">
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="primary"></b-avatar>
            <span class="mr-auto">Team Member 1</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="primary"></b-avatar>
            <span class="mr-auto">Team Member 2</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="primary"></b-avatar>
            <span class="mr-auto">Team Member 3</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
        </b-list-group>
      </div>
    </b-col>
    <b-col>
      <div>
        <p><strong>Performance Team</strong><p />
        <div class="Kreisbilder">
          <b-avatar variant="danger"></b-avatar>
          <b-avatar variant="warning"></b-avatar>
          <b-avatar variant="info"></b-avatar>
        </div>
        <b-list-group style="max-width: 300px;">
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="warning"></b-avatar>
            <span class="mr-auto">  Team Member 1</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="warning"></b-avatar>
            <span class="mr-auto">  Team Member 2</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
          <b-list-group-item class="d-flex align-items-center">
            <b-avatar variant="warning"></b-avatar>
            <span class="mr-auto">  Team Member 3</span>
            <b-badge>Jobtitle</b-badge>
          </b-list-group-item>
        </b-list-group>
      </div>
    </b-col>
    <b-col>
      <div>
        <p><strong>Creative Team</strong><p />
        <div class="Kreisbilder">
          <b-avatar variant="dark"></b-avatar>
          <b-avatar variant="light"></b-avatar>
          <b-avatar variant="success"></b-avatar>
        </div>
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
    </b-col>
  </b-row>
</template>

<script>
export default {}
</script>

<style scoped>
.Avatare {
    margin-top: 10rem;
    margin-bottom: 4rem;
}
.Kreisbilder {
    margin-bottom: 2rem;
}
</style>
