<template>
    <main>
    <NuxtLink to="/blog">&lt; Back</NuxtLink>
    <h1>
      {{ post.title }}
    </h1>
    <p>{{ post.description }}</p>
    <hr>
    <ContentDoc />
  </main>
</template>

<script setup>
const route = useRoute()

const actualPath = route.path.replace(/\/$/, '');

const { data: post } = await useAsyncData(`hello`, () =>
    queryContent(actualPath).findOne()
);
</script>
