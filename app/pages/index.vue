<script setup lang="ts">
import Carousel from "~/components/carousel.vue";
</script>
<template>
  <section
    class="flex flex-row justify-between w-full my-5 bg-gray-800 pl-10 pr-18 mt-10 pt-20"
  >
    <div class="flex flex-col justify-between w-1/2">
      <div class="w-full">
        <Carousel />
      </div>
      <div>
        <button class="w-11/12 rounded-md h-10 bg-amber-50 text-black mb-4">
          Download
        </button>
        <p>Available on iOS and Android devices</p>
      </div>
    </div>

    <div class="w-1/2 grid-cols-2 grid grid-rows-2 gap-4 p -10">
      <span class="rounded-md bg-white p-0.5">
        <img src="~/assets/images/1.png" alt="Discover Nuxt" />
      </span>
      <span class="rounded-md bg-white p-0.5">
        <img src="~/assets/images/2.png" alt="Discover Nuxt"
      /></span>
      <span class="rounded-md bg-white p-0.5">
        <img src="~/assets/images/4.png" alt="Discover Nuxt"
      /></span>
      <span class="rounded-md bg-white p-0.5">
        <img src="~/assets/images/3.png" alt="Discover Nuxt"
      /></span>
    </div>
  </section>
</template>
