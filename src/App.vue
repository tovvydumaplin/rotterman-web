<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from '@/components/layout/Navbar.vue'
</script>

<template>
  <Header />
  <main>
    <RouterView />
  </main>

</template>
