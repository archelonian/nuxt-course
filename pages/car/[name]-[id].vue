<template>
  <div>
    <div>
      <CarDetailHero />
      <CarDetailAttributes />
      <CarDetailDescription />
      <CarDetailContact />
    </div>
  </div>
</template>

<script setup>
const route = useRoute()
const { toTitleCase } = useUtilities()
useHead({
  title: toTitleCase(route.params.name)
})

definePageMeta({
  layout: "custom"
})
</script>
