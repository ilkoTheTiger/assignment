<template>
  <div>
    <header>
      <nav>
        <nuxt-link to="/home">Home</nuxt-link>
        <nuxt-link to="/posts">Posts</nuxt-link>
        <!-- <nuxt-link to="/posts/{id}"></nuxt-link> -->
      </nav>
    </header>
    <main>
      <NuxtPage />
    </main>
    <footer>All Rights Reserved! &copy; 2023</footer>
  </div>
</template>

<script>
import HomePage from "~/pages/home.vue";
import PostsPage from "~/pages/posts.vue";

export default {
  components: {
    HomePage,
    PostsPage,
  },
};
</script>
