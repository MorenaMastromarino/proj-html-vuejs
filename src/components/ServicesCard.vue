<template>
  <div class="col-4">
    <div class="single-card">

      <div class="card-icons d-flex justify-content-between">
        <img :src="require(`../assets/img/${cardData.icon}`)" alt=""> 

        <div>
          <i class="fas fa-arrow-right"></i>
        </div>
      </div> 

      <h4>{{cardData.title}}</h4>

      <p class="subtitle">
        {{cardData.text}}
      </p>

    </div>
  </div>
</template>

<script>
export default {
  name: 'ServicesCard',
  props: {
    cardData: Object,
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';


.single-card {
  height: 100%;
  border-radius: 5px;
  padding: 45px 50px 60px 50px;
  background-color: #fff;
  &:hover i {
    border-radius: 50%;
    background-color: rgba($primary-color, .4);
  }
  img {
    width: 50px;
    margin-bottom: 30px;
    filter: $primary-color-filter;
  }
  i {
    cursor: pointer;
    padding: 5px;
    font-size: 22px;
    color: lighten($primary-color, 5%);
  }
  h4 {
    margin-bottom: 30px;
    font-size: 26px;
    font-weight: bold;
  }
} 
</style>