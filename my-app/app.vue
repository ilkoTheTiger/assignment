<script setup>
const { data: posts } = await useFetch(
  "https://jsonplaceholder.typicode.com/posts/"
);

// Importing Navigation and Footer Components
import Navigation from "~/components/navigation.vue";
import FooterComponent from "~/components/footer.vue";
</script>

<template>
  <div class="flex flex-col h-screen justify-between">
    <header
      class="border-b bg-gradient-to-r from-sky-500 to-indigo-500 border-gray-300 mb-3"
    >
      <Navigation />
    </header>
    <main class="font-serif p-6 mb-auto">
      <NuxtPage />
      <div v-for="post in posts">
        <ul>
          <li>
            {{ posts }}
          </li>
        </ul>
      </div>
    </main>
    <footer>
      <FooterComponent />
    </footer>
  </div>
</template>
