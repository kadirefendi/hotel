<template>
  <footer class="p-[76px] mx-auto w-[960px]">
    <div id="search-header" class="flex items-center ml-12">
      <span class="uppercase text-4xl mr-6">find</span>
      <div class="inline m-4">
        <span
          class="text-base font-semibold mr-8 cursor-pointer border-black border-b-2"
          >Rooms</span
        >
        <span class="text-base font-semibold mr-8 cursor-pointer">Flats</span>
        <span class="text-base font-semibold mr-8 cursor-pointer">Hostels</span>
        <span class="text-base font-semibold cursor-pointer">Villas</span>
      </div>
    </div>
    <div id="search-bar" class="pl-8 bg-white w-full h-16 rounded-full">
      <div class="">
        <div class="flex flex-row">
          <div class="m-2 pr-2 border-r">
            <span class="block text-sm font-medium">Location</span>
            <input
              type="text"
              name="text"
              class="placeholder-slate-400 focus:outline-none block w-full sm:text-sm"
              placeholder="Which city do you prefer?"
            />
          </div>

          <div class="m-2 pr-2 border-r">
            <span class="block text-sm font-medium">Check In</span>
            <input
              type="text"
              name="date"
              class="placeholder-slate-400 focus:outline-none block w-full sm:text-sm"
              placeholder="Add Dates"
            />
          </div>
          <div class="m-2 pr-2 border-r">
            <span class="block text-sm font-medium">Check Out</span>
            <input
              type="text"
              name="date"
              class="placeholder-slate-400 focus:outline-none block w-full sm:text-sm"
              placeholder="Add Dates"
            />
          </div>
          <div class="m-2 pr-2 border-r">
            <span class="block text-sm font-medium">Guests</span>
            <input
              type="text"
              name="date"
              class="placeholder-slate-400 focus:outline-none block w-full sm:text-sm"
              placeholder="Add Guests"
            />
          </div>
          <div class="flex items-center">
            <span class="material-icons text-3xl"> search </span>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
