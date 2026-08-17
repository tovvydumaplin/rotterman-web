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
<div
    class="
        mt-12.5
        grid
        grid-cols-1
        gap-15
        lg:grid-cols-2
        lg:gap-25
        lg:min-h-100
    "
>
    <!-- Discovery Icon -->
    <div class="order-1 flex justify-center lg:order-1 lg:justify-end">
        Icon
    </div>

    <!-- Discovery Text -->
    <div class="order-2 w-full text-center lg:order-2 lg:w-96.75 lg:text-left">
        <h3 class="text-3xl font-bold text-white!">
            DISCOVERY
        </h3>

        <p class="mt-5 text-white">
            We learn your business inside out — your workflows, your pain points,
            your goals. No assumptions, no guesswork, just deep listening.
        </p>
    </div>


    <!-- Blueprint Text -->
    <div class="order-4 w-full text-center lg:order-3 lg:ml-auto lg:w-84.25 lg:text-right">
        <h3 class="text-3xl font-bold text-white!">
            BLUEPRINT
        </h3>

        <p class="mt-5 text-white">
            We design your system architecture, user flows,
            and UI mockups.
        </p>
    </div>

    <!-- Blueprint Icon -->
    <div class="order-3 flex justify-center lg:order-4 lg:justify-start">
        Icon
    </div>


    <!-- Build Icon -->
    <div class="order-5 flex justify-center lg:order-5 lg:justify-end">
        Icon
    </div>

    <!-- Build Text -->
    <div class="order-6 w-full text-center lg:order-6 lg:w-96.75 lg:text-left">
        <h3 class="text-3xl font-bold text-white!">
            BUILD
        </h3>

        <p class="mt-5 text-white">
            Our developers build and rigorously test your solution.
            Regular check-ins keep you in the loop at every milestone —
            no surprises.
        </p>
    </div>


    <!-- Launch & Support Text -->
    <div class="order-8 w-full text-center lg:order-7 lg:ml-auto lg:w-84.25 lg:text-right">
        <h3 class="text-3xl font-bold text-white!">
            LAUNCH & SUPPORT
        </h3>

        <p class="mt-5 text-white">
            We deploy your system, train your team, and remain your
            dedicated support partner.
        </p>
    </div>

    <!-- Launch & Support Icon -->
    <div class="order-7 flex justify-center lg:order-8 lg:justify-start">
        Icon
    </div>
</div>
        </AppContainer>
    </section>
</template>