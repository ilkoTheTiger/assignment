<template>
  <article class="post w-full p-7 rounded-xl">
    <h2 class="w-full text-2xl mb-2 text-gray-700 flex justify-between">
      <span>Check our our Latest Blog Posts</span>
    </h2>
    <div v-for="num in 3" class="backdrop-blur-2xl rounded-xl py-3 px-5 my-4">
      <h2 class="w-full text-2xl mb-2 text-gray-700 flex justify-between">
        <span>Lorem ipsum? Dolore?</span>
        <span>#{{ 541 - num }}</span>
      </h2>
      <p class="mt-1 text-gray-600 text-xl">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
        officia, nesciunt dicta ipsam culpa natus suscipit accusamus ipsa nam
        vel harum possimus quod cupiditate quam ratione, alias veniam dolore id.
      </p>
    </div>
  </article>
</template>
