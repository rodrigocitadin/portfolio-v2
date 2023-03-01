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
  <div class="bg-neutral-50 text-neutral-800 font-light h-screen text-lg">
    <header>
      <AboutMe />
    </header>
    <main>
      <TitleLink divTitle="books I've read" :links="links" />
      <TitleLink divTitle="writings" :links="links" />
      <TitleLink divTitle="skills" :links="links" />
    </main>
  </div>
</template>
