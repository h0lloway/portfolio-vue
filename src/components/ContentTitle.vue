<script setup>
  const props = defineProps({
    title: {
      type: String,
      default: 'Title'
    }
  })
</script>

<template>
  <h2 class="heading-2">{{ title }}</h2>
</template>