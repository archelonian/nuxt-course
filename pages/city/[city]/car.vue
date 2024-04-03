<template>
  <div>
    <div class="mt-32 flex">
      <CarSidebar />
      <NuxtPage />
    </div>
  </div>
</template>

<script setup>
const route = useRoute()
useHead({
  title: `${route.params.make ? route.params.make + 's' : 'Cars'} in ${route.params.city}`
})

definePageMeta({
  layout: "custom"
})
</script>
