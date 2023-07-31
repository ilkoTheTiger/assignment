<template>
  <div>
    <header>
      <nav>
        <li><a href="/home" class="">Home</a></li>
        <li><a href="/posts" class="">Home</a></li>
        <li><a href="/home" class="">Home</a></li>
      </nav>
    </header>
    <main>
      <HomePage />
    </main>

  </div>
</template>


<script>
    import HomePage from '~/pages/home.vue'

    export default {
        components: {
            HomePage
        }
    }
</script>