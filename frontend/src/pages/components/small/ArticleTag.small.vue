
<script setup lang="ts">

defineProps<{ tag: string }>()

</script>


<template>
    <a href="#" class="tag">{{ tag }}</a>
</template>


<style scoped>
.tag {
    font-size: 0.7em;
    font-weight: 600;
    border: 1px solid var(--text);
    padding: 5px;
    border-radius: 5px;
    text-decoration: none;
    color: var(--text);
    margin: 5px;
}


.tag:hover {
    color: var(--primary);
    border-color: var(--primary);
    cursor: pointer;
}


</style>