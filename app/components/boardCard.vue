<script setup lang="ts">
const props = defineProps<{
  name: string;
  position: string;
  bio: string;
}>();
</script>

<template>
  <div
    class="bg-gray-50 space-y-3 p-4 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <p class="font-semibold text-lg">{{ name }}</p>
    <p class="font-medium">{{ position }}</p>
    <p class="text-gray-500">{{ bio }}</p>
  </div>
</template>
