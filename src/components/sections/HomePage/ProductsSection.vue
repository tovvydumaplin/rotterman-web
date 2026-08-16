<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
import { ArrowRight } from 'lucide-vue-next'
    const products = [
    {
        id: '01',
        title: 'RALE ERP',
        description:
        'A next-generation enterprise resource planning platform that unifies operations, inventory, finance, and logistics into one breathing system built for Filipino SMEs.',
        tags: ['ERP', 'SAAS', 'DASHBOARD'],
    },
    {
        id: '02',
        title: 'RALE HRIS',
        description:
        'Full-spectrum HR information system covering talent acquisition, performance cycles, payroll processing, and employee lifecycle management.',
        tags: ['HRIS', 'PAYROLL', 'WORKFORCE'],
    },
    {
        id: '03',
        title: 'RALE IMS',
        description:
        'Intelligent inventory management with real-time stock tracking, automated reorder alerts, multi-warehouse support, and supplier management.',
        tags: ['INVENTORY', 'WAREHOUSE', 'TRACKING'],
    },
    {
        id: '04',
        title: 'RALE FINANCE',
        description:
        'Intelligent financial management with real-time reporting, budget forecasting, scenario modeling, and compliance-ready accounting tools.',
        tags: ['FINANCE', 'ACCOUNTING', 'REPORTING'],
    },
    ]

</script>
<template>
    <section>
        <AppContainer>
            <div class="py-30">
                <div>
                    <h5 class="text-sm">
                        OUR PRODUCT / MEET RALE
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
                        What we’ve
                        <span class="primary-color">
                        Built.
                        </span>
                    </h2>
                </div>
                    <div
                        v-for="product in products"
                        :key="product.id"
                        class="
                            grid

                            grid-cols-[1fr_40px]
                            gap-x-4
                            gap-y-5
                            py-8

                            lg:grid-cols-[60px_220px_1fr_250px_40px]
                            lg:items-center
                            lg:gap-8
                            lg:py-10

                            border-b
                            border-gray-200
                        
                        "
                    >
                        <!-- Number -->
                        <span class="
                                hidden
                                lg:block

                                text-sm
                                self-start
                                lg:self-auto
                        ">
                        {{ product.id }}
                        </span>

                        <!-- Title -->
                        <h3 class="
                            text-2xl
                            sm:text-3xl
                            font-bold

                            col-span-1

                            lg:col-span-1
                        
                        ">
                        {{ product.title }}
                        </h3>

                        <!-- Description -->
                        <p class="
                            col-span-3
                            text-gray-600
                            text-sm
                            sm:text-base
                            leading-relaxed

                            lg:col-span-1
                        
                        ">
                        {{ product.description }}
                        </p>

                        <!-- Tags -->
                        <div class="
                                col-start-1
                                flex
                                flex-wrap
                                gap-x-4
                                gap-y-2
                                text-xs
                                uppercase

                                lg:col-start-auto
                                lg:justify-end
                                lg:gap-4
                        ">
                        <span
                            v-for="tag in product.tags"
                            :key="tag"
                        >
                            {{ tag }}
                        </span>
                        </div>

                        <!-- Arrow -->
                        <button class="
                                col-start-3
                                justify-self-end
                                self-end
                                text-2xl

                                lg:col-start-auto
                                lg:row-start-auto
                                lg:self-auto
                        
                        ">
                        <ArrowRight :size="20" />
                        </button>
                    </div>
            </div>
        </AppContainer>
    </section>
</template>