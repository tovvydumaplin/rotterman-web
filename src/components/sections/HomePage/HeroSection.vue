<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import Header from '@/components/layout/Navbar.vue'
import BaseButton from '@/components/ui/BaseButton.vue';
import heroImage from '@/assets/images/hero-image.png'

</script>

<template>
  <section class="min-h-screen relative gap-4 md:gap-6 lg:gap-8 xl:gap-10 overflow-hidden bg-[#F7F7F0]">
    <AppContainer>
      <Header />
      <div class="grid grid-cols-2 gap-8 py-30">
        <!-- Left -->
        <div>
          <h5 class="text-sm">
            custom software for filipino smes
          </h5>

          <h1 class="
            font-heading 
            font-semibold
            mt-2 
            text-4xl
            md:text-5xl
            lg:text-6xl
            xl:text-7xl
            2xl:text-8xl"
            >
            DIGITAL SOLUTIONS
            <span class="primary-color">
              BUILT AROUND YOUR BUSINESS
            </span>
          </h1>

          <p class="mt-5 max-w-xl text-md">
            We build custom ERP, HRIS, POS, and business management systems that help Filipino companies automate workflows, improve efficiency, and scale faster.
          </p>

          <div class="mt-10 flex gap-4">
            <BaseButton 
                variant="primary" 
                size="lg"
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
              class="w-full h-auto scale-120 translate-x-10"
            />
        </div>

      </div>
    </AppContainer>
  </section>
</template>
<style scoped></style>
