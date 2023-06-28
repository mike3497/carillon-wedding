<template>
  <nav class="container mx-auto pt-2 pb-4">
    <div class="flex items-center justify-between">
      <!-- Mobile menu button -->
      <div class="flex md:hidden">
        <button
          type="button"
          class="text-zinc-800 hover:text-zinc-400 focus:outline-none focus:text-zinc-400 p-2"
          @click="showMenu = !showMenu"
        >
          <i class="fa-solid fa-bars"></i>
        </button>
      </div>
    </div>
    <ul
      :class="showMenu ? 'flex' : 'hidden'"
      class="flex-col md:flex md:flex-row md:items-center gap-4"
    >
      <li>
        <NuxtLink to="/" activeClass="text-zinc-800">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/our-story" activeClass="text-zinc-800"
          >Our Story</NuxtLink
        >
      </li>
      <li>
        <NuxtLink to="/photos" activeClass="text-zinc-800">Photos</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/registry" activeClass="text-zinc-800">Registry</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/wedding-details" activeClass="text-zinc-800"
          >Wedding Details</NuxtLink
        >
      </li>
    </ul>
  </nav>
</template>

<script setup lang="ts">
const showMenu = ref<boolean>(false);
</script>

<!-- <template>
  <nav class="flex flex-row text-zinc-500">
    <NuxtLink class="m-2" to="/" activeClass="text-zinc-800">Home</NuxtLink>
    <NuxtLink class="m-2" to="/" activeClass="text-zinc-800"
      >Our Story</NuxtLink
    >
    <NuxtLink class="m-2" to="/" activeClass="text-zinc-800">Photos</NuxtLink>
    <NuxtLink class="m-2" to="/" activeClass="text-zinc-800">Registry</NuxtLink>
    <NuxtLink class="m-2" to="/" activeClass="text-zinc-800"
      >Wedding Details</NuxtLink
    >
  </nav>
</template> -->
