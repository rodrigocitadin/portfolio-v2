<template>
  <div class="max-w-3xl mx-auto mt-8">
    <div class="mx-8">
      <h2 class="text-xl font-bold">{{ divTitle }}</h2>
    </div>
    <div class="mx-8">
      <ul>
        <li v-for="link in links" :key="link.name">
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
export type Link = {
  name: string
  value: string
}

defineProps<{
  divTitle: string
  links: Link[]
}>()
</script>
