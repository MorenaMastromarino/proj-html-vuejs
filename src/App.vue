<template>
  <div>
    <Header />
    <Jumbotron :menuData=jumboMenuData />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Jumbotron from './components/Jumbotron.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Footer
  },
  data(){
    return{
      jumboMenuData: [
        'home',
        'services',
        'about',
        'projects',
        'results'
      ]
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/vars.scss';
@import './assets/style/general.scss';
@import './assets/style/utilities.scss';

</style>
