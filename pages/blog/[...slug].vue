<template>
    <article class="prose dark:prose-invert 
    prose-pre:bg-white 
    dark:prose-pre:bg-gray-800 
    prose-pre:text-gray-700 
    dark:prose-pre:text-gray-300
    max-w-none">
        <ContentDoc v-slot="{ doc }">
           

            <div class="grid grid-cols-6 gap-16">
                <div :class="{ 'col-span-4': doc.toc, 'col-span-6': !doc.toc}">
                    <ContentRenderer :value="doc" />
                    
                </div>
                <div class="col-span-2 not-prose" v-if="doc.toc">
                <aside class="sticky top-8">
                    <div class="font-semibold mb-2">
                        Table of Content
                    </div>
                    <nav>
                        <TocLinks :links="doc.body.toc.links" />
                    </nav>
                </aside>
            </div>
            </div>
        </ContentDoc>
    </article>
    <div>
    
    </div>
</template>

<script setup>
const route =useRoute()
console.log(route.params.slug)
</script>