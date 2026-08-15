<script setup>
    import AppContainer from '@/components/ui/AppContainer.vue';
    import LogoImageWhite from '@/assets/images/logo-white.png'
    import { RouterLink} from 'vue-router'
</script>
<template>
    <section class="bg-[#071609] pt-30">
        <AppContainer>

            <div class="flex justify-between">
                <!-- LOGO  -->
                <div class="logo-box">
                    <img
                    :src="LogoImageWhite"
                    alt="Logo"
                    class="h-8 md:h-10 lg:h-12 xl:h-14 w-auto"
                    />
                </div>
                <!-- FOOTER MENUS  -->
                <div class="footer-menus flex gap-25">
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
                    <div class="location">
                        <h5 class="text-sm text-[#B9B9B9]!">Location</h5>
                        <nav class="flex flex-col gap-5 mt-7.5">
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                Philippines Laguna
                            </RouterLink>
                        </nav>
                    </div>
                    <div class="contact">
                        <h5 class="text-sm text-[#B9B9B9]!">Contact</h5>
                        <nav class="flex flex-col gap-5 mt-7.5">
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                rotterman@example.com
                            </RouterLink>
                            <RouterLink
                                to="/"
                                class="text-white hover:text-[#186534] transition duration-300"
                                >
                                +63 93238512313
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