<template>
  <main>      

      <!-- services -->
      <section class="services mm-py">

        <div class="container">
          <!-- titolo -->
          <div class="services-title">
            <h6 class="top-title">Our business areas</h6>
            <h2>
              Excellence in 
              <span class="highlighted">Services</span>
            </h2>

            <div class="services-title-bottom d-flex justify-content-between">
              <p class="subtitle">
                We are leaders in providing consultancy services with a set of cutting-eedge technologies and a team of experienced and renowned professionals. These are some options that you can hire.
              </p>

              <div>
                <button type="button" class="btn mm-btn-green">
                  see all       
                </button>
              </div>
            </div>

          </div>

          <!-- cards -->
          <div class="row g-4">
            
            <ServicesCard
              v-for="(servicesCard, index) in servicesCardsData" 
              :key="`servicesCard${index}`"
              :cardData="servicesCard"
            />
            
          </div>
          
        </div>

      </section>

      <!-- about -->
      <!-- projects -->
      <!-- results -->
      <!-- get in touch -->
  </main>
</template>

<script>
import ServicesCard from './ServicesCard.vue';

export default {
  name: 'Main',
  components: {
    ServicesCard,

  },
  data(){
    return {
      servicesCardsData: [
        {
          icon: 'svg-1.svg',
          title: 'Audit & Asuurance',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
        {
          icon: 'svg-2.svg',
          title: 'Financial Advisory',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
        {
          icon: 'svg-3.svg',
          title: 'Analytics and M&A',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
        {
          icon: 'svg-4.svg',
          title: 'Middle Marketing',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
        {
          icon: 'svg-5.svg',
          title: 'Legal Consulting',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
        {
          icon: 'svg-6.svg',
          title: 'Regulatory Risk',
          text: 'Lorem ipsum dolor sit amet consectetur adipiscing elit.'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

/*** services ***/
.services {
  background-color: #EEF4ED;
  .services-title {
    margin-bottom: 50px;
    .subtitle {
      width: 75%;
    }
  }

}


</style>