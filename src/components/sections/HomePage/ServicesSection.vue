<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
</script>
<template>
    <section class="bg-[#F7F7F0] py-30">
        <AppContainer>
                <div>
                    <h5 class="text-sm">
                        Services / WHAT WE DO
                    </h5>

                    <h2 class="
                        font-semibold
                        mt-2 
                        text-2xl
                        md:text-3xl
                        lg:text-4xl
                        xl:text-5xl
                        2xl:text-6xl"
                        >
                        Services for your
                        <span class="primary-color">
                        Business.
                        </span>
                    </h2>
                </div>
                <div class="grid grid-cols-[1.3fr_0.7fr] gap-7.5 mt-12.5">
                    <div class="p-7.5 border border-[#186534] rounded">
                        <div
                            class="w-full h-58 bg-gray-200 rounded-lg flex items-center justify-center mb-6"
                        >
                            <span class="text-gray-500 text-sm">
                                Image Placeholder
                            </span>
                        </div>
                        <h3 class="text-3xl font-bold">Custom WEB APPLICATIONS</h3>
                        <p class="mt-5 text-md">Tailored portals, dashboards, and management platforms built from scratch around your unique workflows — not the other way around.</p>
                        <div class="border-t border-gray-300 pt-5 mt-7.5">
                               
                        </div>
                    </div>
                    <div class="flex flex-col gap-7.5">
                        <div class="flex-1 p-7.5 border border-[#186534] rounded">
                            <h3 class="text-3xl font-bold">UI/ux DESIGN</h3>
                        </div>
                        <div class="flex-1 p-7.5 border border-[#186534] rounded ">
                            <h3 class="text-3xl font-bold">UI/ux DESIGN</h3>
                        </div>
                    </div>
                </div>
                
        </AppContainer>
    </section>


</template>