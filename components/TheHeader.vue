<template>
  <header class="bg-white shadow">
    <div class="container mx-auto px-4">
      <div class="flex flex-row justify-between text-xs py-4">
        <ul class="flex flex-row">
          <li>July 22, 2023</li>
          <li class="mx-2">|</li>
          <li>Cleveland, OH</li>
        </ul>
        <p>#CarillonWeddingBells</p>
      </div>
      <div class="flex flex-row items-center justify-center">
        <img src="/assets/images/title-left.png" />
        <h1 class="font-display text-center text-4xl">Katherine & Michael</h1>
        <img src="/assets/images/title-right.png" />
      </div>
      <TheNavbar />
    </div>
  </header>
</template>

<script setup lang="ts">
import TheNavbar from '../components/TheNavbar.vue';
</script>
