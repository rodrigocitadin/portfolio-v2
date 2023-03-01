<script setup lang="ts">
import AboutMe from './components/AboutMe.vue'
import TitleLink from './components/TitleLink.vue'
import type { Link } from './components/TitleLink.vue'

const books: Link[] = [
  { name: 'Typescript Handbook', value: 'https://www.typescriptlang.org/docs/handbook/intro.html' },
  { name: 'The Prince - Niccolo Machiavelli', value: 'https://www.amazon.com.br/Prince-Niccolo-Machiavelli/dp/0140449159' },
  { name: 'The Art Of War', value: 'https://www.amazon.com/Art-War-Sun-Tzu/dp/1599869772' },
  { name: 'Discipline Is Destiny: The Power of Self-Control', value: 'https://www.amazon.com.br/Discipline-Destiny-Self-Control-Ryan-Holiday/dp/0593191692' }
]

const contributed: Link[] = [
  {name: 'elixir4noobs', value: 'https://github.com/aleDsz/elixir4noobs'},
  {name: 'he4rtoberfest 2022', value: 'https://github.com/he4rt/he4rtoberfest-2022'}
]

const skills: Link[] = [
  { name: 'Typescript', value: '#' },
  { name: 'NodeJs', value: '#' },
  { name: 'Vue', value: '#' },
  { name: 'Rust', value: '#' },
  { name: 'Elixir', value: '#' },
  { name: 'Mathematics', value: '#' },
  { name: 'Functional Programming', value: '#' },
  { name: 'Git', value: '#' },
  { name: 'Postgres', value: '#' },
  { name: 'MongoDB', value: '#' },
  { name: 'Redis', value: '#' },
  { name: 'Docker', value: '#' },
]
</script>

<template>
  <div class="bg-neutral-50 text-neutral-800 font-light min-h-screen text-base">
    <header>
      <AboutMe />
    </header>
    <main>
      <TitleLink divTitle="books I've read" :links="books" />
      <TitleLink divTitle="I've contributed to" :links="contributed" />
      <TitleLink divTitle="skills" :links="skills" />
    </main>
  </div>
</template>
