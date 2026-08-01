<script setup>
defineProps({
  betlogByRicky: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1 class="text-green-500 text-6xl">{{ betlogByRicky }}</h1>
  </div>
</template>

<style scoped></style>
