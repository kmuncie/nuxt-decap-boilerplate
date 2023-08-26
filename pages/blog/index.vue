<template>
  <main>
    <h1>The Blog</h1>
    <hr>
    <ul>
      <li v-for="post of posts" :key="post.slug">
        <NuxtLink :to="post._path">{{ post.title }}</NuxtLink>
      </li>
    </ul>
  </main>
</template>

<script setup>
const { data: posts } = await useAsyncData('posts', () => {
  return queryContent('/blog').find()
})
</script>
