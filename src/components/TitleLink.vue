<template>
  <div>
    <div>
      <h2>{{ divTitle }}</h2>
    </div>
    <div>
      <ul>
        <li v-for="link in links" :key="link.name">
          <a :href="link.value">{{ link.name }}</a>
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
