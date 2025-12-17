<script setup lang="ts">
import Carousel from "~/components/carousel.vue";
</script>
<template>
  <section
    class="flex md:flex-row flex-col justify-between w-full bg-gray-800 md:pl-10 md:pr-18 pt-30"
  >
    <div class="flex flex-col justify-between w-full md:w-1/2 gap-y-3">
      <div class="w-full px-4">
        <Carousel />
      </div>
      <div class="flex flex-col text-white gap-y-4 mb-10 pl-4">
        <NuxtLink
          class="w-11/12 rounded-md h-10 bg-gray-100 text-black mb-4 flex items-center justify-center font-medium"
          to="www.neocash.ng"
        >
          <img
            src="~/assets/images/download_2.png"
            alt="download Logo"
            class="h-5 mx-3 inline-block mt-2"
          />
          Download
        </NuxtLink>
        <p class="mb-3">Available on iOS and Android devices</p>

        <div class="flex flex-row w-full h-20 gap-x-6 items-center px-5 my-4">
          <span>
            <img src="~/assets/images/cbn.png" alt="CBN Logo" class="h-10" />
          </span>
          <span>
            <img src="~/assets/images/ndic.png" alt="NDIC Logo" class="h-10" />
          </span>
          <p class="w-3/5">
            Licensed by the Central Bank of Nigeria. All deposits are insured by
            the Nigeria Deposit Insurance Corporation.
          </p>
        </div>
      </div>
    </div>

    <div class="md:w-1/2 w-full">
      <div class="h-24 hidden md:block" />
      <div class="grid-cols-2 grid grid-rows-2 gap-4 p-3">
        <img
          src="~/assets/images/1.png"
          alt="Discover Nuxt"
          class="border border-amber-50 rounded-md"
        />

        <img
          src="~/assets/images/2.png"
          alt="Discover Nuxt"
          class="border border-amber-50 rounded-md"
        />
        <img
          src="~/assets/images/3.png"
          alt="Discover Nuxt"
          class="border border-amber-50 rounded-md"
        />
        <img
          src="~/assets/images/4.png"
          alt="Discover Nuxt"
          class="border border-amber-50 rounded-md"
        />
      </div>
    </div>
  </section>
  <Hero1 />
  <Hero2 />
  <Hero3 />
</template>
