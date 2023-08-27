<template>
  <NuxtPage />
</template>

<script setup>
useHead({
  title: 'Nuxt Decap Boilerplate',
  meta: [
    { name: 'description', content: 'A simple boilerplate site.' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})
</script>

<style lang="scss">
@use "~/assets/scss/collector.scss";
</style>
