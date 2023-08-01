<script setup>
// Importing Navigation and Footer Components
import Navigation from "~/components/navigation.vue";
import FooterComponent from "~/components/footer.vue";
</script>

<template>
  <div class="flex flex-col h-screen justify-between">
    <header
      class="border-b bg-gradient-to-r from-sky-400 to-indigo-400 border-gray-200"
    >
      <Navigation />
    </header>
    <main
      class="font-serif p-6 mb-auto bg-gradient-to-r from-sky-500 to-indigo-500"
    >
      <NuxtPage />
    </main>
    <footer>
      <FooterComponent />
    </footer>
  </div>
</template>
