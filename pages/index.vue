<template>
    <div>
        Hello from main page
    </div>
</template>
<script setup>
useSeoMeta({
    title: 'Main Page',
    description: 'This is the main page',
    ogTitle: 'Main Page',
    ogDescription: '[og:description]',
    ogImage: '[og:image]',
    ogUrl: '[og:url]',
    twitterTitle: 'MainPage',
    twitterDescription: '[twitter:description]',
    twitterImage: '[twitter:image]',
    twitterCard: 'summary'
  })
  
  useHead({
    htmlAttrs: {
      lang: 'en'
    },
  link: [
      {
        rel: 'icon',
        type: 'image/x-icon',
        href: '/favicon.ico'
      }
    ]
  })
</script>