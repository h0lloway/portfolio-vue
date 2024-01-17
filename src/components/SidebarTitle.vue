<script setup>
  const props = defineProps({
    title: {
      type: String,
      default: 'Title'
    }
  })
</script>

<template>
  <h5 class="heading-5">{{ title }}</h5>
</template>