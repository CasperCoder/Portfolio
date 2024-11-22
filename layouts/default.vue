<template>
    <div class="container mx-auto">
        <header class="flex justify-between items-center mt-5">
           <div class="flex items-center space-x-12">
            <div>
<NuxtLink to="/" class="text-xl font-semivold p-2 hover:bg-gray-200 dark:hover:bg-gray-600">Kacper Zagrodziński</NuxtLink>

            </div>

       <Menu />
           </div>
           <ClientOnly>
             <ColorModeSelector />

           </ClientOnly>
</header>
        0 references
    <main class="p-2 mt-10">

        <slot />
    </main> 
    </div>
</template>

<script setup>


useHead({
  titleTemplate: '%s - Kacper I Zagrodziński',
  

  link: [
    {
      rel: 'preconnect',
      href: 'https://fonts.googleapis.com'
    },
    {
      rel: 'stylesheet',
      href: 'https://fonts.googleapis.com/css2?family=Roboto&display=swap',
      crossorigin: ''
    }
  ]
})
</script>

<style>
body {
  font-family: 'Roboto';
}

body {
  @apply bg-white dark:bg-gray-900 text-gray-700 dark:text-gray-300
}
</style>