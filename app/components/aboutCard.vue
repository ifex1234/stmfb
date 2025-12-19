<script setup lang="ts">
const props = defineProps<{
  imageSrc: string;
  title: string;
  description: string;
  listItms?: string[];
  paragraphItems?: string[];
}>();
</script>
<template>
  <div
    class="shadow-md p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <span class="flex flex-row space-x-3">
      <img v-bind:src="imageSrc" alt="" />
      <h2 class="text-2xl font-semibold mb-2">{{ title }}</h2>
    </span>

    <p class="text-gray-600 mb-4">{{ description }}</p>
    <ul
      v-if="listItms && listItms.length"
      class="list-disc list-inside text-gray-600"
    >
      <li v-for="(item, index) in listItms" :key="index">{{ item }}</li>
    </ul>
    <div v-if="paragraphItems && paragraphItems.length" class="space-y-2">
      <p
        v-for="(para, index) in paragraphItems"
        :key="index"
        class="text-gray-600"
      >
        {{ para }}
      </p>
    </div>
  </div>
</template>
