<template>
  <div class="max-w-3xl mx-auto">
    <div class="mx-8">
      <h1 class="pt-16 font-bold text-xl">
        Hi, I'm Citadin
      </h1>
      <p class="w-4/5 mt-4">
        fullstack developer, focused in backend, mathematics, type systems, and functional programming.
      </p>
    </div>
    <div class="mx-8">
      <ul class="mt-8">
        <li class="mt-2" v-for="link in links" :key="link.name">
          <a
            class="underline decoration-2 decoration-neutral-400 hover:decoration-black"
            target="_blank"
            :href="link.value"
          >
            {{ link.name }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup lang="ts">
import type { Link } from './TitleLink.vue';

const links: Link[] = [
  { name: "linkedin", value: "https://www.linkedin.com/in/rodrigobcitadin/" },
  { name: "github", value: "https://github.com/rodrigocitadin/" },
  { name: "dev.to", value: "https://dev.to/rodrigocitadin" }
]
</script>
