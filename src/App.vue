<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
</script>

<template>
  <div class="">
    <div
      class="flex flex-col justify-between h-screen w-full bg-[url('./assets/kumtano.jpg')] bg-cover"
    >
      <Header />
      <Footer />
    </div>
    <div class="h-screen w-max-[1280px]">
      <div class="mx-12 mt-12">
        <div class="">
          <span class="block text-4xl">Latest on the </span>
          <span class="text-4xl">Property Listing</span>
          <hr class="w-24 border-2 border-black mt-4" />
        </div>
        <div class="flex flex-row">
          <div class="basis-1/4 bg-slate-400 h-80 mr-4">hey</div>
          <div class="basis-1/4 bg-slate-400 h-80 mr-4">hey</div>
          <div class="basis-1/4 bg-slate-400 h-80 mr-4">hey</div>
          <div class="basis-1/4 bg-slate-400 h-80">hey</div>
        </div>
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
</style>
