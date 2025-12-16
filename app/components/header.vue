<template>
  <nav
    class="bg-white flex justify-between h-14 items-center text-black md:px-10 w-full"
  >
    <div
      class="flex items-center flex-row gap-2 px-3 w-full md:w-2/3 justify-between md:justify-start"
    >
      <div class="flex justify-start items-center">
        <span class="font-semibold text-xl mr-3">Shepherd Trust </span>
        <span class="text-gray-400 text-sm">Microfinance Bank</span>
      </div>
      <span class="block md:hidden"><Drawer /></span>
    </div>
    <div
      class="md:flex w-1/3 justify-between text-sm font-medium pr-8 hidden gap-3"
    >
      <NuxtLink
        class="hover:bg-gray-200 h-10 w-16 hover:rounded-md place-content-center flex items-center"
        to="/"
        >Home</NuxtLink
      >
      <NuxtLink
        class="hover:bg-gray-200 h-10 w-16 hover:rounded-md place-content-center flex items-center"
        to="/about"
        active-class="bg-gray-200 font-bold rounded-md"
        >About</NuxtLink
      >
      <NuxtLink
        class="hover:bg-gray-200 h-10 w-16 hover:rounded-md place-content-center flex items-center"
        to="/services"
        active-class="bg-gray-200 font-bold rounded-md"
        >Services</NuxtLink
      >
      <NuxtLink
        class="hover:bg-gray-200 h-10 w-16 hover:rounded-md place-content-center flex items-center"
        to="/careers"
        active-class="bg-gray-200 font-bold rounded-md"
        >Careers</NuxtLink
      >
      <NuxtLink
        class="hover:bg-gray-200 h-10 w-16 hover:rounded-md place-content-center flex items-center"
        to="/contact"
        active-class="bg-gray-200 font-bold rounded-md"
        >Contact</NuxtLink
      >
    </div>
  </nav>
</template>
