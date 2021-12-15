<template>
  <div class="jumbotron">

    <!-- top -->
    <div class="container d-flex justify-content-between align-items-center mt-4">
      

      <div class="logo">
        <img src="../assets/img/svg-7.svg" alt="logo">
      </div>

      <div class="jumbo-menu">
        <nav class="d-inline-block">
          <ul class="m-0">
            <li v-for="(data,index) in menuData" :key="index">
              <a href="#">{{data}}</a>
            </li>
          </ul>
        </nav>

        <button type="button" class="btn mm-btn-green">Get in touch</button>
        
      </div>
      
    </div>

    <!-- center -->
    <div class="jumbo-title text-center">
      <h1>
        Ready 
        <span class="highlighted">Team</span>
      </h1>
      <p class="subtitle">
        No matter what your company needs, we will be ready to assist you in the best possible way.
      </p>

      <button type="button" class="btn mm-btn-green">
        Get in touch        
      </button>
      <button type="button" class="btn mm-btn-white">
        Read more        
      </button>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Jumbotron',
  props: {
    menuData: Array,
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.jumbotron {
  position: relative;
  height: calc(100vh - 50px);
  width: 100%;
  background-image: url(../assets/img/bg-parallax.png);
  background-position: center;

  /* top */
  .logo {
    width: 150px;
    img {
      width: 100%;
    }
  }
  nav li {
    display: inline-block;
    padding: 18px;
    text-transform: uppercase;
    color: $secondary-color;    
  }

  /* center */
  .jumbo-title {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 35%;
    transform: translate(-50%, -50%);
    h1 {
      margin-bottom: 30px;
      font-size: 70px;      
    }
    p {
      margin-bottom: 50px;
    }
    .mm-btn-green {
      margin-right: 25px;
    }
  }
  
}

</style>