<template>
  <div class="mx-12 mt-12">
    <div class="">
      <span class="block text-4xl">Latest on the </span>
      <span class="text-4xl">Property Listing</span>
      <hr class="w-24 border-2 border-black mt-4 mb-4" />
    </div>
    <div class="flex flex-row">
      <div
        class="flex flex-col justify-end basis-1/4 bg-slate-400 h-80 mr-4"
        v-for="hotel in hotels"
        :key="hotel"
      >
        <div class="flex flex-col m-4">
          <span class="text-lg font-semibold text-slate-100 mb-2">{{
            hotel.type
          }}</span>
          <!-- {{ hotel.caption }} -->
          <span class="text-sm text-slate-200">{{ hotel.name }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import axios from 'axios'
import { ref } from 'vue'

const hotels = ref([])

const options = {
  method: 'GET',
  url: 'https://hotels4.p.rapidapi.com/locations/v2/search',
  params: { query: 'new york', locale: 'en_US', currency: 'USD' },
  headers: {
    'X-RapidAPI-Host': 'hotels4.p.rapidapi.com',
    'X-RapidAPI-Key': 'bdd13eb543mshb641c8572dea658p1c5b03jsn8290602773bf',
  },
}

axios
  .request(options)
  .then(function (res) {
    console.log(res.data.suggestions)
    // console.log('first =>', res.data.suggestions[1].entities)
    hotels.value = res.data.suggestions[1].entities
  })
  .catch(function (error) {
    console.error(error)
  })
</script>
