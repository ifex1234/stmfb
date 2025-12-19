<script setup lang="ts">
const props = defineProps<{
  name: string;
  position: string;
  imageSrc: string;
  bio: string;
}>();
</script>
<template>
  <div
    class="shadow-md flex gap-y-2 justify-center flex-col items-center p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <Placeholder class="h-8" />
    <img
      :src="imageSrc"
      alt=""
      class="w-28 h-28 rounded-[100%] object-cover mb-4"
    />
    <h2 class="text-2xl font-semibold mb-2">{{ name }}</h2>
    <h3 class="text-xl text-gray-600 mb-4">{{ position }}</h3>
    <p class="text-gray-600 text-center">{{ bio }}</p>
    <NuxtLink
      to="/"
      class="hover:bg-gray-200 cursor-pointer place-content-center text-center h-10 w-full outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
      >Connect on Linkedin</NuxtLink
    >
  </div>
</template>
