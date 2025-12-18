<script setup lang="ts">
defineProps<{
  title: string;
  listItems: string[];
}>();
</script>
<template>
  <div
    class="p-2 md:p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <h4 class="md:text-2xl text-xl font-medium mb-4">{{ title }}</h4>

    <ul v-if="listItems" class="list-disc list-inside space-y-2">
      <li v-for="(item, index) in listItems" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>
