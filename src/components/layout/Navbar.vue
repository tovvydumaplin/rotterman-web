<template>
  <header class="w-full">
    <div
      class="
        flex
        items-center
        justify-between
        py-5
      "
    >

      <!-- Logo -->
      <RouterLink to="/" class="shrink-0">
        <img
          :src="LogoImage"
          alt="Logo"
          class="
            h-8
            md:h-10
            lg:h-12
            w-auto
          "
        />
      </RouterLink>


      <!-- Desktop Navigation -->
      <nav
        class="
          hidden
          lg:flex
          items-center
          gap-6
          xl:gap-10
        "
      >
        <RouterLink
          to="/about"
          class="
            text-gray-900
            font-medium
            hover:text-[#186534]
            transition-colors
            duration-300
          "
        >
          About
        </RouterLink>

        <RouterLink
          to="/services"
          class="
            text-gray-900
            font-medium
            hover:text-[#186534]
            transition-colors
            duration-300
          "
        >
          Services
        </RouterLink>

        <RouterLink
          to="/products"
          class="
            text-gray-900
            font-medium
            hover:text-[#186534]
            transition-colors
            duration-300
          "
        >
          Products
        </RouterLink>

        <RouterLink
          to="/pricing"
          class="
            text-gray-900
            font-medium
            hover:text-[#186534]
            transition-colors
            duration-300
          "
        >
          Pricing
        </RouterLink>

        <RouterLink
          to="/contact"
          class="
            text-gray-900
            font-medium
            hover:text-[#186534]
            transition-colors
            duration-300
          "
        >
          Contact
        </RouterLink>
      </nav>


      <!-- Desktop Button -->
      <div class="hidden lg:block">
        <BaseButton
          variant="primary"
          size="md"
          @click="goToPreviousTab"
        >
          Get Started
        </BaseButton>
      </div>


      <!-- Mobile Menu Button -->
      <button
        class="
          lg:hidden
          flex
          items-center
          justify-center
          gap-2
          h-10
          px-3
          rounded
          border
          border-[#186534]
        "
        aria-label="Open menu"
      >
          <Menu :size="20" />
          <span class="text-sm font-medium uppercase">
            Menu
          </span>
      </button>

    </div>
  </header>
</template>
<script setup>
import { RouterLink} from 'vue-router'
import LogoImage from '@/assets/images/rotterman-logo.png'
import BaseButton from '@/components/ui/BaseButton.vue';
import { Menu } from 'lucide-vue-next'
</script>