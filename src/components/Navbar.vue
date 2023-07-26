<template>
  <nav class="nav">
    <div class="container">
      <a href="#"><img src="src/assets/img/logo.svg" alt="" class="logo"></a>
      <ul class="nav_list">
        <li><a href="#about" class="nav_link">About</a></li>
        <li><a href="#service" class="nav_link">Services</a></li>
        <li><a href="#portfolio" class="nav_link">Portfolio</a></li>
        <li><a href="#contact" class="nav_link">Contact</a></li>
      </ul>
      <div class="hamburger">
        <input type="checkbox" id="checkbox" @click="burger">
        <label for="checkbox" class="toggle">
          <div class="bars" id="bar1"></div>
          <div class="bars" id="bar2"></div>
          <div class="bars" id="bar3"></div>
        </label>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const burger = ref(() => {
  const list = document.querySelector('.nav_list');
  list.classList.toggle('resp');
})
</script>

<style lang="scss" scoped></style>