<script setup lang="ts">
const items = [
  {
    header: "Rewarding savers with high returns",
    content:
      " For over a decade, we've helped traders, small businesses, and growing enterprises access the funding they need to thrive. Now, with ourdigital solutions, we're making it even easier to bank with us.",
  },
  {
    header: "Evolving lenders with improved collection",
    content:
      " For over a decade, we've helped traders, small businesses, and growing enterprises access the funding they need to thrive. Now, with our digital solutions, we're making it even easier to bank with us.",
  },
  {
    header: "Empowering Nigerian businesses with accessible finance",
    content:
      " For over a decade, we've helped traders, small businesses, and growing enterprises access the funding they need to thrive. Now, with our digital solutions, we're making it even easier to bank with us.",
  },
];
</script>

<template>
  <UCarousel
    v-slot="{ item }"
    loop
    :autoplay="{ delay: 4000 }"
    :items="items"
    :ui="{ item: 'basis-1/1' }"
  >
    <div class="flex flex-col justify-between h-full gap-y-6 pr-10">
      <p class="w-full h-3/4 rounded-lg font-semibold text-5xl">
        {{ item["header"] }}
      </p>
      <p class="font-semibold text-lg w-full h-1/4">
        {{ item["content"] }}
      </p>
    </div>
  </UCarousel>
</template>
