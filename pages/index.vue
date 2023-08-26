<script setup>

useHead({
  title: 'Home',
  script: [
    { src: "https://identity.netlify.com/v1/netlify-identity-widget.js" },
  ]
});

</script>
<template>
  <main>
    <h1>Welcome!</h1>
    <hr>
      <p>This template demonstrates the creation of a static site using:</p>
      <ul>
        <li>Nuxt 3</li>
        <li>Decap CMS (formerly Netlify)</li>
      </ul>
      <h2>The Blog</h2>
      <p>The blog is the core of this site. <NuxtLink to="/blog">Click here -></NuxtLink></p>
  </main>
</template>
