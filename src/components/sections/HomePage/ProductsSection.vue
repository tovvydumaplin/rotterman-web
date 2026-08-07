<script setup>
import AppContainer from '@/components/ui/AppContainer.vue';
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
                        class="grid grid-cols-[60px_220px_1fr_250px_40px] items-center gap-8 border-b border-gray-200 py-10"
                    >
                        <!-- Number -->
                        <span class="text-sm">
                        {{ product.id }}
                        </span>

                        <!-- Title -->
                        <h3 class="text-3xl font-bold">
                        {{ product.title }}
                        </h3>

                        <!-- Description -->
                        <p class="text-gray-600">
                        {{ product.description }}
                        </p>

                        <!-- Tags -->
                        <div class="flex justify-end gap-4 text-xs uppercase">
                        <span
                            v-for="tag in product.tags"
                            :key="tag"
                        >
                            {{ tag }}
                        </span>
                        </div>

                        <!-- Arrow -->
                        <button class="text-2xl">
                        ↗
                        </button>
                    </div>



            </div>
        </AppContainer>
    </section>
</template>