<template>
  <div id="app">

    <!-- <img src="./assets/logo.png"> -->

    <app--navigation></app--navigation> 
    <app--slider></app--slider>

    <app--cont--1></app--cont--1>
    

    <app--footer></app--footer>

    
  </div>
</template>

<script>
import Navigation from "components/Navigation.vue";
import Slider from "components/Slider.vue";
import Footer from "components/Footer.vue";

import Content_1 from "components/Content_1.vue";

export default {
  name: "app",
  components: {
    "app--navigation": Navigation,
    "app--slider": Slider,
    "app--footer": Footer,
    "app--cont--1": Content_1
  }
};
</script>

<style>
</style>
