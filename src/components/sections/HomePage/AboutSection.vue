<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import BaseButton from '@/components/ui/BaseButton.vue';
import AboutImage from '@/assets/images/about-image.png'

</script>

<template>
  <section class="relative gap-4 md:gap-6 lg:gap-8 xl:gap-10 overflow-hidden py-30">
    <AppContainer>
      <div class="grid grid-cols-2 items-center gap-25">
        <!-- Left -->
        <div class="w-full">
            <img
              :src="AboutImage"
              alt="Hero"
              class="w-full h-auto scale-120 -translate-x-10"
            />
        </div>

        <!-- Right -->
        <div>
          <h5 class="text-sm">
            About Rotterman
          </h5>

          <h2 class="
            font-semibold
            mt-2 
            text-2xl
            md:text-3xl
            lg:text-4xl
            xl:text-6xl
            2xl:text-7xl"
            >
            Proudly filipino.
            <span class="primary-color">
              BUIlt for local businesess.
            </span>
          </h2>

          <p class="mt-5 max-w-xl text-md">
            We are a Filipino software company dedicated to helping local SMEs embrace digital. From fully custom management systems to our ready-to-use RALE enterprise suite — we build tools tailored to how you actually work.
          </p>

          <div class="mt-10 flex gap-4">
            <BaseButton 
                variant="primary" 
                size="lg"
                @click="goToPreviousTab"
            >
                See How We Build
            </BaseButton>
            <BaseButton 
                variant="secondary" 
                size="lg"
                @click="goToPreviousTab"
            >
                Learn About Us
            </BaseButton>
          </div>
        </div>
      </div>
    </AppContainer>
  </section>
</template>
<style scoped></style>
