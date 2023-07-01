<script setup>
import Header from './components/Header.vue';
import Info from './components/Info.vue';
import Schedule from './components/Schedule.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />
  <Info />
  <div class="vectors">
    <div class="wrapper">
      <img class="" src="@/components/icons/hidden-vector.svg" alt="">
      <img class="" src="@/components/icons/vector.svg" alt="">
      <img class="" src="@/components/icons/vector.svg" alt="">
    </div>

    <div class="wrapper">
      <img class="" src="@/components/icons/vector.svg" alt="">
      <img class="" src="@/components/icons/last-vector.svg" alt="">

    </div>
  </div>
  <Schedule />
  <img class="pexels-wendy" src="@\assets\pexels-wendy.jpg" alt="">
  <Contact />
  <Footer />
</template>

<style scoped>
  .vectors {
    display: flex;
    justify-content: space-between;
    margin-top: 2em;
    margin-bottom: 2em;
  }

  .pexels-wendy {
    width: 100%;
    height: auto;
    padding-top: 3em;
  }

  @media (max-width: 1000px) {
    .vectors img {
      height: 100px;
    }
  }
  @media (max-width: 500px) {
    .vectors img {
      height: 60px;
    }

    .vectors {
      margin: 0;
    }
  }
</style>
