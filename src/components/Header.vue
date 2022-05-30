<template>
  <header class="flex justify-between py-5 px-[76px]">
    <div id="logo">
      <img
        alt="Vue logo"
        class="logo"
        src="@/assets/logo.svg"
        width="40"
        height="40"
      />
    </div>

    <div>
      <nav class="inline">
        <RouterLink to="/" class="mr-3 text-base font-semibold"
          >Find a Property</RouterLink
        >
        <RouterLink to="/about" class="mr-5 text-base font-semibold"
          >Share Stories</RouterLink
        >
        <RouterLink to="/about" class="mr-5 text-base font-semibold"
          >Rental Guides</RouterLink
        >
        <RouterLink to="/about" class="mr-5 text-base font-semibold"
          >Download App</RouterLink
        >
      </nav>

      <button class="bg-slate-600 px-4 py-1 rounded-full ml-8">
        <span class="text-white">Become a Host</span>
      </button>
    </div>

    <div id="initial">Options</div>
  </header>
</template>
