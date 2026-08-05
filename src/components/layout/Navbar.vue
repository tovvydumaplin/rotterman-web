<template>
  <header class="w-full">
    <div class="flex justify-between py-5">

      <!-- Logo -->
      <div class="flex items-center">
        <img
          :src="LogoImage"
          alt="Logo"
          class="h-6 md:h-8 lg:h-10 xl:h-12 w-auto"
        />
      </div>

      <!-- Navigation -->
      <nav class="flex items-center gap-10">
        <RouterLink
          to="/"
          class="text-gray-900 font-medium hover:text-[#186534] transition duration-300"
        >
          About
        </RouterLink>

        <RouterLink
          to="/about"
          class="text-gray-900 font-medium hover:text-[#186534] transition duration-300"
        >
          Services
        </RouterLink>

        <RouterLink
          to="/services"
          class="text-gray-900 font-medium hover:text-[#186534] transition duration-300"
        >
          Products
        </RouterLink>

        <RouterLink
          to="/contact"
          class="text-gray-900 font-medium hover:text-[#186534] transition duration-300"
        >
          Pricing
        </RouterLink>
        <RouterLink
          to="/contact"
          class="text-gray-900 font-medium hover:text-[#186534] transition duration-300"
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