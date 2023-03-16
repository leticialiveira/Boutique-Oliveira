<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import HeaderVue from './components/HeaderVue.vue'
import SectionSlide from './components/MainVue.vue'
import SectionShopping from './components/SectionShopping.vue'
import SectionShopping2 from './components/SectionShopping2.vue'
import SectionVideo from './components/SectionVideo.vue'
import SectionVideo2 from './components/SectionVideo2.vue'
import SectionFooter from './components/SectionFooter.vue'
</script>

<template>
  <header>
    <HeaderVue />
  </header>
  <section class="section-slide">
    <h1>Novidades:</h1>
    <SectionSlide />
  </section>
  <section class="section-shopping">
    <SectionShopping />
  </section>
  <section class="section-shopping">
    <SectionShopping2 />
  </section>
  <section class="section-shopping">
    <SectionVideo />
  </section>
  <section class="section-shopping">
    <SectionVideo2 />
  </section>
  <section class="section-footer">
    <SectionFooter />
  </section>

  </template>
  <!-- <RouterView /> -->

<style scoped>
 header { 
    width: 80vw;
    height: 120px;
    background-color: #CB954F;
    /* border-radius: 10px; */
    display: flex;
    align-items: center;
    font-family: 'Cinzel', cursive;
    font-weight: 400;
    margin: 10px auto 0;
    /* justify-content: center; */
}

.section-slide {
    display: flex;
    align-items: center;
    margin: 0px auto 0;
    background-color:#FFECD2;
    width: 80vw;
    height: 650px;
    font-family: 'Cinzel', serif;
    flex-direction: column;
    gap: 30px;
    /* border-radius: 8px; */

}

.section-slide h1 {
  margin-top: 10px;
  color:#4F2D00;
  font-size: xx-large;
}

.section-shopping {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 80vw;
  height: 700px;
  background-color:#FFECD2;
  margin: 0px auto 0;
  gap: 500px;
  border-top: solid 1px #4F2D00;

}

.section-footer { 
    width: 80vw;
    height: auto;
    background-color: #CB954F;
    display: flex;
    /* border-radius: 10px; */
    align-items: center;
    font-family: 'Cinzel', cursive;
    font-weight: 400;
    margin: 0px auto 0;
    padding: 10px;
}
</style>
