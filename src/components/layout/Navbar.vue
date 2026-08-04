<template>
  <header class="w-full">
    <div class="max-w-7xl flex justify-between py-5">

      <!-- Logo -->
      <div class="flex items-center">
        <img
          :src="LogoImage"
          alt="Logo"
          class="h-10 w-auto"
        />
      </div>

      <!-- Navigation -->
      <nav class="flex items-center gap-10">
        <RouterLink
          to="/"
          class="text-gray-700 hover:text-blue-600 transition duration-300"
        >
          Home
        </RouterLink>

        <RouterLink
          to="/about"
          class="text-gray-700 hover:text-blue-600 transition duration-300"
        >
          About
        </RouterLink>

        <RouterLink
          to="/services"
          class="text-gray-700 hover:text-blue-600 transition duration-300"
        >
          Services
        </RouterLink>

        <RouterLink
          to="/contact"
          class="text-gray-700 hover:text-blue-600 transition duration-300"
        >
          Contact
        </RouterLink>
      </nav>

      <!-- Button -->
      <div>
        <BaseButton
            variant="primary" 
            size="md"
            @click="goToPreviousTab"
        >
            Get Started
        </BaseButton>
      </div>

    </div>
  </header>
</template>
<script setup>
import { RouterLink} from 'vue-router'
import LogoImage from '@/assets/images/logo.png'
import BaseButton from '@/components/ui/BaseButton.vue';
</script>