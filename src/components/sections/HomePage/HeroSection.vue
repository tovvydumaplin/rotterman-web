<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import Header from '@/components/layout/Navbar.vue'
import BaseButton from '@/components/ui/BaseButton.vue';
import heroImage from '@/assets/images/hero-image.png'

</script>

<template>
  <section class="relative overflow-hidden bg-[#F7F7F0]">
    <AppContainer>
      <Header />
      <div class="grid grid-cols-2 gap-8 py-30">
        <!-- Left -->
        <div>
          <h5 class="text-sm">
            custom software for filipino smes
          </h5>

          <h1 class="font-heading mt-2 text-8xl font-bold leading-none">
            DIGITAL SOLUTIONS
            <span class="primary-color">
              BUILT AROUND YOUR BUSINESS
            </span>
          </h1>

          <p class="mt-6 max-w-xl text-md">
            We build custom ERP, HRIS, POS, and business management systems that help Filipino companies automate workflows, improve efficiency, and scale faster.
          </p>

          <div class="mt-10 flex gap-4">
            <BaseButton 
                variant="primary" 
                size="md"
                @click="goToPreviousTab"
            >
                Let’s Build Your System
            </BaseButton>

            <BaseButton 
                variant="secondary" 
                size="md"
                @click="goToPreviousTab"
            >
                Let’s Build Your System
            </BaseButton>
          </div>
        </div>


        <!-- Right -->
        <div class="flex justify-center">
            <img
              :src="heroImage"
              alt="Hero"
              class="w-full h-auto object-cover scale-120 translate-x-10"
            />
        </div>

      </div>
    </AppContainer>
  </section>
</template>
<style scoped></style>
