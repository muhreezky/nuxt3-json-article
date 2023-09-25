<template>
  <NuxtLayout>
    <nuxt-page />
  </NuxtLayout>
</template>

<script lang="ts" setup>
  useHead({
    title: 'Artikel Nuxt',
    meta: [
      { name: 'description', content: 'Artikel JSON Nuxt.js 3' },
      { name: 'og:title', content: 'Artikel Nuxt.js' },
      { name: 'title', content: 'Nuxt.js Article' }
    ],
  })
</script>