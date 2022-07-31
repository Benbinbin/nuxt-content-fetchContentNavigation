<script setup lang="ts">
const queryBuilder = queryContent('sub-folder')
const { data: tree } = await useAsyncData('tree', () => fetchContentNavigation(queryBuilder))
console.log(tree)
</script>

<template>
  <main>
    <ContentDoc />
  </main>
</template>
