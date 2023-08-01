<template>
  <div class="backdrop-blur-2xl hover:bg-gray-100 rounded-xl py-3 px-5 my-2">
    <h2 class="w-full text-2xl mb-2 text-gray-700 flex justify-between">
      <span>{{ post.title }}</span>
      <span>#{{ post.id }}</span>
    </h2>

    <p class="mt-1 text-gray-600 text-xl">
      {{ post.body }}
    </p>
  </div>
</template>

<script>
export default {
  props: ["post"],
};
</script>
