<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import BaseButton from '@/components/ui/BaseButton.vue';
import AboutImage from '@/assets/images/about-image.png'

</script>

<template>
  <section class="relative gap-4 md:gap-6 lg:gap-8 xl:gap-10 overflow-hidden py-20 xl:py-30">
    <AppContainer>
      <div class="
            grid 
            grid-cols-1 
            lg:grid-cols-2
            items-center 
            gap-25"
      >
        <!-- Left -->
        <div class=" 
              w-full
              flex
              justify-center
              mt-4
              lg:mt-0

              order-2
              lg:order-1
              "
              >
            <img
              :src="AboutImage"
              alt="Hero"
              class="
              w-96
              lg:w-112.5
              xl:w-full


              h-auto 
              scale-120 
              lg:-translate-x-4
              xl:-translate-x-8
              2xl:-translate-x-10
              "
            />
        </div>

        <!-- Right -->
        <div class="
              text-center 
              lg:text-left
        
              order-1
              lg:order-2
        ">

            <h5 class="text-sm">
                About Rotterman
            </h5>

            <h2
                class="
                    font-semibold
                    mt-2
                    text-4xl
                    lg:text-5xl
                    xl:text-6xl
                    2xl:text-7xl
                "
            >
                Proudly Filipino.
                <span class="primary-color">
                    Built for local businesses.
                </span>
            </h2>

            <p
                class="
                    mt-5
                    max-w-xl
                    mx-auto
                    lg:mx-0
                    text-md
                "
            >
                We are a Filipino software company dedicated to helping local SMEs
                embrace digital. From fully custom management systems to our
                ready-to-use RALE enterprise suite — we build tools tailored to
                how you actually work.
            </p>

            <div
                class="
                    mt-10
                    flex
                    flex-col
                    items-center
                    sm:flex-row
                    justify-center
                    lg:justify-start
                    gap-4
                "
            >
                <BaseButton
                    variant="primary"
                    size="md"
                    @click="goToPreviousTab"
                >
                    See How We Build
                </BaseButton>

                <BaseButton
                    variant="secondary"
                    size="md"
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
