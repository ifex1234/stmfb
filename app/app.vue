<script setup lang="ts">
import Header from "./components/header.vue";
</script>
<template>
  <div>
    <NuxtLayout>
      <UApp>
        <Header />
        <NuxtPage />
      </UApp>
    </NuxtLayout>
  </div>
</template>
