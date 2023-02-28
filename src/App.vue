<script setup lang="ts">
import AboutMe from './components/AboutMe.vue'
import TitleLink from './components/TitleLink.vue'
import type { Link } from './components/TitleLink.vue'

const links: Link[] = [
  { name: 'a', value: '#' },
  { name: 'b', value: '#' },
  { name: 'c', value: '#' },
]
</script>

<template>
  <div class="bg-amber-50 h-screen text-neutral-900">
    <header>
      <AboutMe />
    </header>
    <main>
      <TitleLink divTitle="books I've read" :links="links" />
    </main>
  </div>
</template>

<style>
* {
    border: 1px solid red;
  }
</style>
