<template>
  <div class="Hero container">
    <b-row>
      <b-col>
        <div class="text-container">
          <h1 class="header">Integr8</h1>
          <h3 class="subtitle">Organigramm</h3>
          <p class="snippet">Lorem ipsum dolor sit amet, con adipisicing elit. Iste iusto illum quidem asperiores, cum nisi aperiam eius ipsa sapiente odit!</p>
        </div>
      </b-col>
      <b-col>
        <img src="data:image/png;base64,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" class="image" alt="i8">
      </b-col>
    </b-row>
    <b-form-select v-model="selected" :options="options" size="m" class="mt-3"/>
    <div class="mt-3">Selected: Du hast das Team <strong>{{ selected }}</strong> ausgewählt</div>
  </div>
  <!--<img src="https://www.integr8.com/wp-content/uploads/2021/11/integr8_preview.png"> class="image" alt="i8">-->
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
  }
}
</script>

<style scoped>
    .Hero {
        padding: 3rem 0;
        align-items: flex-start;
        justify-content: space-between;
    }
    .text-container {
        width: 50%;
        margin-top: 4rem;
    }
    .header {
        font-weight: 900;
        font-size: 5rem;
    }
    .subtitle {
        font-weight: 500;
        font-size: 3rem;
    }
    .snippet {
        color: grey;
        font-size: 1.25rem;
    }
    .image {
        width: 16.5rem;
        justify-content: center;
        height: auto;
    }
    @media (max-width: 500px) {
        .Hero {
            height: 40vh;
    }
        }
</style>
