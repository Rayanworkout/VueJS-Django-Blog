<script setup lang="ts">
import ArticleInGrid from './ArticleInGrid.component.vue'

defineProps(['articles', 'state'])

</script>

<template>
    <div class="container py-4">
        <div v-if="state.loading" class="text-center">Loading <span class="cursor">_</span></div>
        <div v-if="articles.length === 0 && !state.error && !state.loading" class="text-center">No article at the moment <span
                class="cursor">_</span></div>
        <div v-if="state.error" class="text-center">Error while fetching the articles ...</div>
        <div v-else>
            <TransitionGroup name="fade2">
                <div v-for="article in articles" :key="article.id">
                    <ArticleInGrid :article="article" />
                </div>
            </TransitionGroup>
        </div>
    </div>
</template>