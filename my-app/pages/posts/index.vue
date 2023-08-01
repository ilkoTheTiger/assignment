<script setup>
const { data: posts } = await useFetch(
  "https://jsonplaceholder.typicode.com/posts/"
);

// Importing PostCard Component
import PostCard from "~/components/PostCard.vue";
</script>

<template>
  <section
    class="backdrop-blur-2xl bg-white/80 max-w-6xl mx-auto flex flex-wrap py-6 px-6 xl:px-0 p-3"
  >
    <h2 class="w-full text-4xl text- flex justify-center justify-items-center">
      Posts
    </h2>
    <article v-for="post in posts" class="post w-full px-7 py-1 rounded-xl">
      <NuxtLink :to="'/posts/' + post.id">
        <PostCard :post="post" />
      </NuxtLink>
    </article>
  </section>
</template>