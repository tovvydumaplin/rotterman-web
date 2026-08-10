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
                    gap-42.5
                    ">
                    <div class="flex justify-end">Icon</div>
                    <div>text</div>
            </div>
        </AppContainer>
    </section>
</template>