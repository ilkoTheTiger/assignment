<script setup>
const { data: posts } = await useFetch(
  "https://jsonplaceholder.typicode.com/posts/"
);
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
        <div
          class="backdrop-blur-2xl hover:bg-gray-100 rounded-xl py-3 px-5 my-2"
        >
          <h2 class="w-full text-2xl mb-2 text-gray-700 flex justify-between">
            <span>{{ post.title }}</span>
            <span>#{{ post.id }}</span>
          </h2>

          <p class="mt-1 text-gray-600 text-xl">
            {{ post.body }}
          </p>
        </div>
      </NuxtLink>
    </article>
  </section>
</template>
