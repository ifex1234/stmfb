<script setup lang="ts">
defineProps<{
  imageURL: string;
  tile: string;
  description: string;
  listItems: string[];
}>();
</script>

<template>
  <div
    class="p-2 md:p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <span class="flex flex-row space-x-3">
      <img v-bind:src="imageURL" alt="" />
      <h4 class="text-lg font-semibold">{{ tile }}</h4>
    </span>

    <p class="text-gray-500 py-3">{{ description }}</p>
    <ul v-if="listItems" class="list-disc list-inside space-y-2 text-gray-500">
      <li v-for="(item, index) in listItems" :key="index">{{ item }}</li>
    </ul>
    <NuxtLink
      to="/www.neochash.ng"
      class="block text-center bg-gray-900 text-white px-4 mt-5 py-2 rounded-md hover:bg-gray-800"
      >Learn more</NuxtLink
    >
  </div>
</template>
