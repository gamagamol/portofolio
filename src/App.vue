<!-- @format -->

<script setup>
import NavbarComponent from './components/NavbarComponent.vue';

</script>

<template>
  <NavbarComponent/>
</template>

<style>
@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}

.infinite-scroll-container {
  position: relative;
  width: 100%;
  overflow: hidden;
}

.infinite-scroll-content {
  display: flex;
  animation: scroll 5s linear infinite;
}

/* Pause animation on hover */
.infinite-scroll-content:hover {
  animation-play-state: paused;
}
</style>
