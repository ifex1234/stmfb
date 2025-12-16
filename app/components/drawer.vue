<template>
  <UDrawer direction="right">
    <UButton color="neutral" variant="solid" trailing-icon="i-lucide-menu" />

    <template #content>
      <div class="min-w-96 min-h-96 size-full m-4 flex flex-col gap-4">
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/about">About</NuxtLink>
        <NuxtLink to="/services">Services</NuxtLink>
        <NuxtLink to="/careers">Careers</NuxtLink>
        <NuxtLink to="/contact">Contact</NuxtLink>
      </div>
    </template>
  </UDrawer>
</template>
