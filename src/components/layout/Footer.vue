<script setup>
    import AppContainer from '@/components/ui/AppContainer.vue';
    import LogoImageWhite from '@/assets/images/rotterman-logo-white.png'
    import { RouterLink} from 'vue-router'
</script>
<template>
    <section class="bg-[#071609] pt-30">
        <AppContainer>

            <div class="flex flex-col lg:flex-row justify-between gap-[80px]">
                <!-- LOGO  -->
                <div class="logo-box">
                    <img
                    :src="LogoImageWhite"
                    alt="Logo"
                    class="h-12 md:h-14 lg:h-16 xl:h-18 w-auto"
                    />
                </div>
                <!-- FOOTER MENUS  -->
                <div class="footer-menus flex gap-37.5">
                    <div class="sitemap">
                        <h5 class="text-sm text-[#B9B9B9]!">Sitemap</h5>
                        <nav class="flex flex-col gap-5 mt-7.5">
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                About
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Services
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Product
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Pricing
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                FAQ
                            </RouterLink>
                        </nav>
                    </div>
                    <div class="legal">
                        <h5 class="text-sm text-[#B9B9B9]!">Legal</h5>
                        <nav class="flex flex-col gap-5 mt-7.5">
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Imprint
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Privacy Policy
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Terms & Conditions
                            </RouterLink>
                        </nav>
                    </div>
                    <div class="social">
                        <h5 class="text-sm text-[#B9B9B9]!">Social</h5>
                        <nav class="flex flex-col gap-5 mt-7.5">
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Linkedin
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Facebook
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Instagram
                            </RouterLink>
                        </nav>
                    </div>
                </div>
            </div>

            <div class="border-t border-[#B9B9B9] mt-30 py-7.5 flex justify-between">
                <h5 class="text-[#B9B9B9]! text-sm">© 2026 - Rotterman. All Rights Reserved.</h5>
                <h5 class="text-[#B9B9B9]! text-sm">BUILT IN PHILIPPINES</h5>
            </div>

        </AppContainer>
    </section>
</template>