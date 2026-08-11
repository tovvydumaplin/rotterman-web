<script setup>
    import AppContainer from '@/components/ui/AppContainer.vue';
    import BaseButton from '@/components/ui/BaseButton.vue';
</script>
<template>
    <section class="py-30 bg-[#F7F7F0]">
        <AppContainer>
            <div class="grid grid-cols-2 items-center gap-25">
                <!-- Left -->
                <div>
                    <h5 class="text-sm">
                        Contact
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
                        Ready to Transform
                        <span class="primary-color">
                        Your Business?
                        </span>
                    </h2>

                    <p class="mt-5 max-w-xl text-md">
                        Tell us about your project and we'll get back to you with a tailored solution.
                    </p>
                    <div class="w-full mt-7.5">
                        <div class="grid grid-cols-[62px_1fr] gap-12.5 border-y border-gray-200 py-5">
                            <h5 class="text-[#B9B9B9]! ">EMAIL</h5>
                            <p>rotterman@example.com</p>
                        </div>
                        <div class="grid grid-cols-[62px_1fr] gap-12.5 border-b border-gray-200 py-5">
                            <h5 class="text-[#B9B9B9]! ">Phone</h5>
                            <p>+63 93238512313</p>
                        </div>
                        <div class="grid grid-cols-[62px_1fr] gap-12.5 border-b border-gray-200 py-5">
                            <h5 class="text-[#B9B9B9]! ">EMAIL</h5>
                            <p>Philippines Laguna</p>
                        </div>
                    </div>
                </div>


                <!-- Right -->
                <div class="w-full bg-[#182423] p-10 rounded-sm">
                    
                </div>
            </div>
        </AppContainer>
    </section>
</template>