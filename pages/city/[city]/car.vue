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
const { toTitleCase } = useUtilities()
useHead({
  title: `${route.params.make
          ? toTitleCase(route.params.make + 's')
          : 'Cars'} in ${toTitleCase(route.params.city)}`
})

definePageMeta({
  layout: "custom"
})
</script>
