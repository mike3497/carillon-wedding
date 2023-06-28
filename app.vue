<template>
  <main>
    <TheHeader />
    <NuxtPage />
    <TheFooter />
  </main>
</template>

<script setup lang="ts">
useHead({
  bodyAttrs: {
    class: 'bg-slate-50',
  },
});
</script>
