<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import Header from '@/components/layout/Navbar.vue'
defineProps({
  betlogByRicky: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <section class="relative overflow-hidden bg-slate-950 text-white">
    <AppContainer>
      <Header />
      <div class="grid grid-cols-2 py-30">

        <!-- Left -->
        <div>
          <span class="text-blue-400">
            Welcome
          </span>

          <h1 class="mt-6 text-5xl font-bold leading-tight lg:text-7xl">
            Build Better
            <span class="text-blue-500">
              Digital Experiences
            </span>
          </h1>

          <p class="mt-6 max-w-xl text-lg text-gray-300">
            Create modern, responsive, and fast websites that help your business grow.
          </p>

          <div class="mt-10 flex gap-4">
            <button
              class="rounded-xl bg-blue-600 px-8 py-4 font-semibold transition hover:bg-blue-700">
              Get Started
            </button>

            <button
              class="rounded-xl border border-white/20 px-8 py-4 font-semibold hover:bg-white/10">
              Learn More
            </button>
          </div>
        </div>


        <!-- Right -->
        <div class="flex justify-center">
          <div class="h-96 w-96 rounded-3xl bg-white/10">
            gg
          </div>
        </div>

      </div>
    </AppContainer>
  </section>
</template>
<style scoped></style>
