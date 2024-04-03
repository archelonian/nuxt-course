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
useHead({
  title: route.params.name
})

definePageMeta({
  layout: "custom"
})
</script>
