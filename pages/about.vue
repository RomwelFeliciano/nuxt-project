<script setup lang="ts">
definePageMeta({
  layout: "authenticated-layout",
});
const counter = useState("counter", () => Math.round(Math.random() * 1000));
</script>

<template>
  <div>
    <div>
      <h1>About page</h1>
      <NuxtLink to="/">Home page</NuxtLink>
    </div>
    <div>
      Counter: {{ counter }}
      <button @click="counter++">+</button>
      <button @click="counter--">-</button>
    </div>
  </div>
</template>
