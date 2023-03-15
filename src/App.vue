<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import HeaderVue from './components/HeaderVue.vue'
import MainVue from './components/MainVue.vue'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
    <HeaderVue />

  </header>
  <section class="section">
    <h1>Novidades:</h1>
    <MainVue />
  </section>
  <section class="section">
  </section>

      

  </template>
  <!-- <RouterView /> -->

<style scoped>
 header { 
    width: 80vw;
    height: 120px;
    background-color: #CB954F;
    border-radius: 10px;
    display: flex;
    align-items: center;
    font-family: 'Amatic SC', cursive;
    font-weight: 400;
    margin: 10px auto 0;
    /* justify-content: center; */
}

.section {
    display: flex;
    align-items: center;
    margin: 0px auto 0;
    background-color:#FFECD2;
    width: 80vw;
    height: 500px;
    font-family: 'Cinzel', serif;
    flex-direction: column;
}

.section h1 {
  margin-top: 10px;
  color:#4F2D00;
  font-size: xx-large;
  text-decoration: underline;
}
/*  
.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  
  .logo {
    margin: 0 2rem 0 0;
  }
  
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  
  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    
    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
