<script setup lang="ts">
const props = defineProps<{
  name: string;
  imageUrl: string;
}>();
</script>

<template>
  <div
    class="flex p-4 gap-y-3 min-h-24 flex-col items-center outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <img :src="imageUrl" alt="" class="h-14" />

    <p class="font-medium text-center">{{ name }}</p>
  </div>
</template>
