<template>
  <div>
    <header class="border-b border-gray-300 mb-3">
      <Navigation />
    </header>
    <main>
      <NuxtPage />
    </main>
    <footer>
      <FooterComponent />
    </footer>
  </div>
</template>

<script>
// Importing Navigation and Footer Components
import Navigation from "~/components/navigation.vue"
import FooterComponent from "~/components/footer.vue";

export default {
  components: {
    Navigation,
    FooterComponent,
  },
};
</script>
