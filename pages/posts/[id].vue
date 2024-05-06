<template>
  <header>
    <nav>
      <ul>
        <li><NuxtLink to="/">About</NuxtLink></li>
        <li><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
        <li><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
      </ul>
      <p>{{ route.params.id }}</p>
    </nav>
  </header>
</template>

<script setup lang="ts">
const route = useRoute();

// When accessing /posts/1, route.params.id will be 1
console.log(route.params);
</script>
