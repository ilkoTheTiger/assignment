<script setup>
// Getting the ID of the Post Dynamically
const { id } = useRoute().params;

// Fetching specific post based on the ID above
const { data: post } = await useFetch(
  `https://jsonplaceholder.typicode.com/posts/${id}`
);
</script>

<template>
  <section
    class="backdrop-blur-2xl bg-white/80 max-w-6xl mx-auto flex flex-wrap py-6 px-6 xl:px-0 p-3 roundex-xl"
  >
    <h2 class="w-full text-4xl text- flex justify-center justify-items-center">
      Post Details
    </h2>
    <article class="post w-full px-7 py-1 rounded-xl">
      <NuxtLink to="/posts">
        <!-- Re-using the Post Card template component and passing the Post Data -->
        <PostCard :post="post" />
      </NuxtLink>
    </article>
  </section>
</template>
