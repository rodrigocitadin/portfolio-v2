<script setup lang="ts">
import AboutMe from './components/AboutMe.vue'
import TitleLink from './components/TitleLink.vue'
import MyFooter from './components/MyFooter.vue'
import type { Link } from './components/TitleLink.vue'

const books: Link[] = [
  { name: 'Typescript Handbook', value: 'https://www.typescriptlang.org/docs/handbook/intro.html' },
  { name: 'The Prince - Niccolo Machiavelli', value: 'https://www.amazon.com.br/Prince-Niccolo-Machiavelli/dp/0140449159' },
  { name: 'The Art Of War', value: 'https://www.amazon.com/Art-War-Sun-Tzu/dp/1599869772' },
  { name: 'Discipline Is Destiny: The Power of Self-Control', value: 'https://www.amazon.com.br/Discipline-Destiny-Self-Control-Ryan-Holiday/dp/0593191692' }
]

const contributed: Link[] = [
  { name: 'elixir4noobs', value: 'https://github.com/aleDsz/elixir4noobs' },
  { name: 'he4rtoberfest 2022', value: 'https://github.com/he4rt/he4rtoberfest-2022' },
]

const skills: Link[] = [
  { name: 'Javascript', value: 'https://www.javascript.com/' },
  { name: 'Typescript', value: 'https://www.typescriptlang.org/' },
  { name: 'Rust', value: 'https://www.rust-lang.org/' },
  { name: 'NodeJs', value: 'https://nodejs.org/en/' },
  { name: 'VueJs', value: 'https://vuejs.org/' },
  { name: 'Mathematics', value: 'https://en.wikipedia.org/wiki/Mathematics' },
  { name: 'Functional Programming', value: 'https://en.wikipedia.org/wiki/Functional_programming' },
  { name: 'Git', value: 'https://git-scm.com/' },
  { name: 'Postgres', value: 'https://www.postgresql.org/' },
  { name: 'MongoDB', value: 'https://www.mongodb.com/' },
  { name: 'Redis', value: 'https://redis.io/' },
  { name: 'Docker', value: 'https://www.docker.com/' },
]
</script>

<template>
  <div class="bg-neutral-50 text-neutral-800 font-light min-h-screen text-base flex flex-col antialiased">
    <div class="flex-1">
      <header>
        <AboutMe />
      </header>
      <main>
        <TitleLink divTitle="books I've read" :links="books" />
        <TitleLink divTitle="I've contributed to" :links="contributed" />
        <TitleLink divTitle="skills" :links="skills" />
      </main>
    </div>
    <footer>
      <MyFooter />
    </footer>
  </div>
</template>
