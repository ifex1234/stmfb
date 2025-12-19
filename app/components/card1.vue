<script setup lang="ts">
defineProps<{
  title: string;
  content: string;
}>();
</script>
<template>
  <div
    class="p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <h4 class="text-2xl font-medium mb-4">{{ title }}</h4>
    <p class="text-gray-500">{{ content }}</p>
  </div>
</template>
