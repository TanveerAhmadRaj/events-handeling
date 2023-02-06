<script setup>
import { RouterView } from 'vue-router'
import Navigation from './components/Navigation.vue';
</script>

<template>
  <div>
    <Navigation />
  </div>

  <RouterView />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800&display=swap');

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Montserrat',
    sans-serif;
  color: #303433;
}

html {

  scroll-behavior: smooth;
  background-color: eee;
}
</style>
