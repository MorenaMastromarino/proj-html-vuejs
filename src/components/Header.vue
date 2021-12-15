<template>
  <header>

    <div class="container h-100 d-flex justify-content-between align-items-center">

      <div class="open-hours">
        <i class="fas fa-clock"></i>
        <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
      </div>

      <div class="contacts">
        <ul class="m-0">
          <li>
            <i class="fas fa-phone-alt"></i>
            <span>+1(305)1234-5678</span>
          </li>
          <li>
            <i class="fas fa-envelope"></i>
            <span>hello@example.com</span>
          </li>
          <li>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
          </li>
          <li>
            <a href="#"><i class="fab fa-twitter"></i></a>
          </li>
          <li>
            <a href="#"><i class="fab fa-linkedin-in"></i></a>
          </li>
        </ul>
      </div>

    </div>

  </header>  
</template>

<script>
export default {
  name: 'Header',

}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

header {
  height: 50px;
  background-color: $secondary-color;
  color: #C0C3D0;
  i {
    padding-right: 7px;
  }
  li {
    display: inline-block;
    padding: 0 15px;
  }
}

</style>