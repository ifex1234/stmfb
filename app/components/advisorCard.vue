<script setup lang="ts">
const props = defineProps<{
  name: string;
  role: string;
  imageUrl: string;
}>();
</script>

<template>
  <div
    class="flex p-4 min-h-24 flex-row gap-5 items-center outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
  >
    <img :src="imageUrl" alt="" class="h-7" />
    <div>
      <p class="font-medium">{{ name }}</p>
      <p class="text-gray-400">{{ role }}</p>
    </div>
  </div>
</template>
