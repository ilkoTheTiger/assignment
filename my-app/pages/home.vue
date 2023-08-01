<script setup>
// Importing Navigation and Footer Components
import LatestCard from "~/components/LatestCard.vue";
</script>

<template>
  <section
    class="backdrop-blur-2xl bg-white/80 max-w-6xl mx-auto flex flex-wrap justify-center py-6 px-6 xl:px-0 p-3"
  >
    <h2 class="w-full text-4xl text- flex justify-center justify-items-center">
      Welcome to our Blog!
    </h2>

    <LatestCard />
    
    <NuxtLink
      to="/posts"
      class="mt-6 inline-block px-8 py-4 rounded-xl bg-blue-500 text-white text-xl hover:bg-blue-700"
    >
      See All Posts
    </NuxtLink>
  </section>
</template>
