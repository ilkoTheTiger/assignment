<script setup>
// Importing Navigation and Footer Components
import Navigation from "~/components/Navigation.vue";
import FooterComponent from "~/components/FooterComponent.vue";
</script>

<template>
  <div
    class="h-max flex flex-col h-screen justify-between bg-gradient-to-r from-sky-500 to-indigo-500"
  >
    <header
      class="border-b bg-gradient-to-r from-sky-400 to-indigo-400 border-gray-200"
    >
      <Navigation />
    </header>

    <main class="min-h-screen font-serif p-6 mb-auto">
      <NuxtPage />
    </main>
    
    <footer class="sticky bottom-0">
      <FooterComponent />
    </footer>
  </div>
</template>
