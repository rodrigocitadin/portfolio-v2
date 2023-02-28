<script setup lang="ts">
const links = [
  'aaa',
  'bbb',
  'ccc',
]
</script>

<template>
  <div>
    <h1>Hello, I'm Citadin</h1>
    <p>I’m a fullstack developer, focused in backend, mathematics, type systems, and functional programming.</p>
    <ul v-for="link in links" :key="link">
      <li><a :href="link">{{ link }}</a></li>
    </ul>
  </div>
</template>

<style scoped></style>
