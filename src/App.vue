<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import PropertyListing from './components/PropertyListing.vue'
</script>

<template>
  <div class="snapper">
    <div
      class="flex flex-col justify-between h-screen w-full bg-[url('./assets/kumtano.jpg')] bg-cover snap-center"
    >
      <Header />
      <Footer />
    </div>
    <div class="h-screen w-full snap-center">
      <div class="h-screen max-w-[1280px] mx-auto">
        <PropertyListing />
      </div>
    </div>
  </div>
  <RouterView />
</template>

<style>
/* @import '@/assets/base.css';
@import '@/assets/app.css'; */

/* .dene:focus {
  border
} */

.snapper {
  overflow: auto;
  scroll-snap-type: y mandatory;
}
</style>
