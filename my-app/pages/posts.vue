<script setup>
const { data: posts } = await useFetch(
  "https://jsonplaceholder.typicode.com/posts/"
);
</script>

<template>
  <div v-for="post in posts">
    <ul>
      <li>
        {{ post.title }}
        {{ post.body }}
      </li>
    </ul>
  </div>
</template>
