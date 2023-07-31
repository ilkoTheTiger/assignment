<template>
  <div>
    <header>
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
import Navigation from "~/components/navigation.vue"
import FooterComponent from "~/components/footer.vue";

export default {
  components: {
    Navigation,
    FooterComponent,
  },
};
</script>
