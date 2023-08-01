<script setup>
const {id} = useRoute().params

const { data: post } = await useFetch(
  `https://jsonplaceholder.typicode.com/posts/${id}`
);
// const id = ref(1);
</script>

<template>
  <h1>{{ $route.params.id }}</h1>
  {{ post }}
</template>
