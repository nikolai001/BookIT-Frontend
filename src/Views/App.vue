<script setup lang="ts">
import { onMounted, ref } from 'vue'

const userIsPresent = ref<boolean>(true)

onMounted(() => {
  setTimeout(() => {
    userIsPresent.value = false
  }, 5000)
})
</script>

<template>
  <h1>Are you awake?</h1>
  {{ userIsPresent }}
</template>
