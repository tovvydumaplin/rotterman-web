<script setup>
    import AppContainer from '@/components/ui/AppContainer.vue';
    const process = [
        {
        id: '01',
        title: 'RALE ERP',
        description:
        'A next-generation enterprise resource planning platform that unifies operations, inventory, finance, and logistics into one breathing system built for Filipino SMEs.',
        }
    ]
</script>
<template>
    <section class="bg-[#071609] py-30">
        <AppContainer>
            <div>
                <h5 class="text-sm text-center text-white!">
                    OUR PROCESS / HOW WE WORK
                </h5>

                <h2 class="
                    text-center
                    font-semibold
                    text-white!
                    mt-2 
                    text-2xl
                    md:text-3xl
                    lg:text-4xl
                    xl:text-5xl
                    2xl:text-6xl"
                    >
                    From BRIEFING  
                    <span class="secondary-color">
                    BRIEFING
                    </span>
                    TO
                    <span class="secondary-color">
                    LAUNCH
                    </span>
                </h2>
            </div>
            <div class="
                    mt-12.5
                    grid
                    grid-cols-1
                    lg:grid-cols-2
                    min-h-100
                    gap-25
                    ">
                    <div class="flex justify-end">Icon</div>
                    <div class="w-96.75">
                        <h3 class="text-3xl font-bold text-white!">DISCOVERY</h3>
                        <p class="mt-5 text-white">We learn your business inside out — your workflows, your pain points, your goals. No assumptions, no guesswork, just deep listening.</p>
                    </div>

                    <div class="w-84.25 ml-auto text-right ">
                        <h3 class="text-3xl font-bold text-white!">
                            BLUEPRINT
                        </h3>

                        <p class="mt-5 text-white">
                            We design your system architecture, user flows,
                            and UI mockups.
                        </p>
                    </div>

                    <div class="flex justify-start">
                        Icon
                    </div>

                    <div class="flex justify-end">Icon</div>

                    <div class="w-96.75">
                        <h3 class="text-3xl font-bold text-white!">Build</h3>
                        <p class="mt-5 text-white">Our developers build and rigorously test your solution. Regular check-ins keep you in the loop at every milestone — no surprises.</p>
                    </div>

                    <div class="w-84.25 ml-auto text-right ">
                        <h3 class="text-3xl font-bold text-white!">
                            Launch & Support
                        </h3>

                        <p class="mt-5 text-white">
                            We deploy your system, train your team, and remain your dedicated support partner.
                        </p>
                    </div>

                    <div class="flex justify-start">
                        Icon
                    </div>
                    
            </div>
        </AppContainer>
    </section>
</template>