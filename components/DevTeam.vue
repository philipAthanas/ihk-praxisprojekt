<template>
  <div class="card-container">
    <b-row>
      <b-col>
        <div>
          <b-card
            no-body
            style="max-width: 15rem"
            img-src="https://www.cmshs-bloggt.de/wp-content/uploads/2017/04/004342_hi-res-600x400.jpg"
            img-alt="Mitarbeiter 1"
            img-top
          >
            <template #header>
              <h4 class="mb-0">i8-Bot No.1</h4>
              <!-- header-text-variant"="white"</>
                #header-bg-variant="dark" -->
            </template>

            <b-card-body>
              <b-card-title>Web-Developer</b-card-title>
              <b-card-sub-title class="mb-2"
                >Kein Plan von nuxtJS</b-card-sub-title
              >
              <b-card-text> Dev-Team </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Verantwortungsbereich</b-list-group-item>
              <b-list-group-item>Aktuelle Projekte</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a
                href="https://de.linkedin.com/company/integr8-media-gmbh"
                class="card-link"
                >Mein LinkedIn-Profil</a
              >
            </b-card-body>

            <b-card-footer>Kontakt Slack</b-card-footer>
          </b-card>
        </div>
      </b-col>
      <b-col>
        <div>
          <b-card
            no-body
            style="max-width: 15rem"
            img-src="https://www.scinexx.de/wp-content/uploads/r/o/roboterg.jpg"
            img-alt="Mitarbeiter 1"
            img-top
          >
            <template #header>
              <h4 class="mb-0">i8-Bot No.2</h4>
            </template>

            <b-card-body>
              <b-card-title>Fullstack Developer</b-card-title>
              <b-card-sub-title class="mb-2"
                >Front- und Backend Pro</b-card-sub-title
              >
              <b-card-text> Dev-Team </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Verantwortungsbereich</b-list-group-item>
              <b-list-group-item>Aktuelle Projekte</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a
                href="https://de.linkedin.com/company/integr8-media-gmbh"
                class="card-link"
                >Mein LinkedIn-Profil</a
              >
            </b-card-body>

            <b-card-footer>Kontakt Slack</b-card-footer>
          </b-card>
        </div>
      </b-col>
      <b-col>
        <div>
          <b-card
            no-body
            style="max-width: 15rem"
            img-src="https://www.mittelstand-heute.com/hubfs/mittelstand-heute_com/blog_images/Titelbild-Roboter-KI-K%C3%BCnstliche-Intelligenz-so-lang-L%C3%A4nge-iStock-543191318-mennovandijk.jpg"
            img-alt="Mitarbeiter 1"
            img-top
          >
            <template #header>
              <h4 class="mb-0">i8-Bot No.3</h4>
            </template>

            <b-card-body>
              <b-card-title>Data Scientist</b-card-title>
              <b-card-sub-title class="mb-2">Big Data Expert</b-card-sub-title>
              <b-card-text> Dev-Team </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Verantwortungsbereich</b-list-group-item>
              <b-list-group-item>Aktuelle Projekte</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a
                href="https://de.linkedin.com/company/integr8-media-gmbh"
                class="card-link"
                >Mein LinkedIn-Profil</a
              >
            </b-card-body>

            <b-card-footer>Kontakt Slack</b-card-footer>
          </b-card>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.card-container {
  img {
    width: 100%;
    height: 200px;
  }
}
</style>
