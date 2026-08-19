<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import BaseButton from '@/components/ui/BaseButton.vue';
import heroImage from '@/assets/images/hero-image.png'


</script>

<template>
  <section class="lg:min-h-screen relative gap-4 md:gap-6 lg:gap-8 xl:gap-10 overflow-hidden bg-[#F7F7F0]">
    <AppContainer>
      <div
        class="
          grid
          grid-cols-1
          lg:grid-cols-2
          items-center
          gap-12
          lg:gap-16
          xl:gap-20
          py-16
          md:py-20
          lg:py-24
          xl:py-30
        "
      >
          <!-- Left -->
          <div class="text-center lg:text-left">

              <h5 class="text-xs sm:text-sm uppercase tracking-wide">
                  Custom software for Filipino SMEs
              </h5>

              <h1
                  class="
                      font-heading
                      font-semibold
                      mt-2

                      text-5xl
                      md:text-6xl
                      lg:text-6xl
                      xl:text-7xl
                      2xl:text-8xl

                      leading-[0.95]
                  "
              >
                  DIGITAL SOLUTIONS
                  <span class="primary-color block">
                      BUILT AROUND YOUR BUSINESS
                  </span>
              </h1>

              <p
                  class="
                      mt-6
                      max-w-xl
                      mx-auto
                      lg:mx-0
                      text-base
                      md:text-lg
                      leading-relaxed
                  "
              >
                  We build custom ERP, HRIS, POS, and business management
                  systems that help Filipino companies automate workflows,
                  improve efficiency, and scale faster.
              </p>

              <div class="mt-8 lg:mt-10 flex justify-center lg:justify-start">
                  <BaseButton
                      variant="primary"
                      size="md"
                      @click="goToPreviousTab"
                  >
                      Let’s Build Your System
                  </BaseButton>
              </div>
          </div>


          <!-- Right -->
          <div
              class="
                    hidden
                    lg:flex
                    justify-center
                    lg:justify-end
                    mt-4
                    lg:mt-0
              "
          >
              <img
                  :src="heroImage"
                  alt="Hero"
                  class="
                     w-[900px]
                     h-auto
                     scale-50
                     
                     lg:scale-100
                     xl:scale-110
                     2xl:scale-125
                      

                      lg:translate-x-4
                      xl:translate-x-8
                      2xl:translate-x-10
                  "
              />
          </div>
          
      </div>
    </AppContainer>
  </section>
</template>
<style scoped></style>
