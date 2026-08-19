<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import { FileCode } from 'lucide-vue-next'
</script>
<template>
    <section class="bg-[#F3F3EF] py-20 xl:py-30">
        <AppContainer>
                <div>
                    <h5 class="text-sm">
                        Services / WHAT WE DO
                    </h5>

                    <h2 class="
                        font-semibold
                        mt-2 
                        text-4xl
                        lg:text-5xl
                        xl:text-6xl
                        2xl:text-7xl
                        "
                        >
                        Services for your
                        <span class="primary-color">
                        Business.
                        </span>
                    </h2>
                </div>
                <div class="
                            grid 
                            grid-cols-1 
                            lg:grid-cols-[1.3fr_0.7fr] 
                            gap-7.5 
                            mt-7.5
                            lg:mt-12.5 
                            ">
                    <div class="p-7.5 border border-[#D5D5D5] rounded bg-white">
                        <div
                            class="w-full h-75 bg-gray-200 rounded-lg flex items-center justify-center mb-6"
                        >
                            <span class="text-gray-500 text-sm">
                                Image Placeholder
                            </span>
                        </div>
                        <h3 class="text-3xl">Custom WEB APPLICATIONS</h3>
                        <p class="mt-5 text-md">Tailored portals, dashboards, and management platforms built from scratch around your unique workflows — not the other way around.</p>
                        <div class="border-t border-gray-300 pt-5 mt-7.5">
                               
                        </div>
                    </div>
                    <div class="flex flex-col gap-7.5 ">
                        <div class="flex-1 p-7.5 border border-[#D5D5D5] rounded bg-white">
                            <div class="inline-flex bg-[#E8F1E9] p-3.75">
                                <FileCode size="20" />
                            </div>
                            <h3 class="mt-7.5 text-3xl ">UI/ux DESIGN</h3>
                            <p class="mt-5 text-md">We create stunning, modern websites tailored to your business. Every design is crafted in Figma, allowing you to review updates.</p>
                        </div>
                        <div class="flex-1 p-7.5 border border-[#D5D5D5] rounded bg-white">
                            <div class="inline-flex bg-[#E8F1E9] p-3.75">
                                <FileCode size="20" />
                            </div>
                            <h3 class="mt-7.5 text-3xl ">WEB DEVELOPMENT</h3>
                            <p class="mt-5 text-md">We build your website from the ground up based on your approved design, using modern development standards and industry best practices.</p>
                        </div>
                    </div>
                </div>
                
        </AppContainer>
    </section>
</template>