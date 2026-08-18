<script setup>
    import AppContainer from '@/components/ui/AppContainer.vue';
    import BaseButton from '@/components/ui/BaseButton.vue';
</script>
<template>
    <section class="py-30 bg-[#F7F7F0]">
        <AppContainer>
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-10 lg:gap-25">
                <!-- Left -->
                <div>
                    <h5 class="text-sm">
                        Contact
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
                            <h5 class="text-sm text-[#B9B9B9]! ">EMAIL</h5>
                            <p>rotterman@example.com</p>
                        </div>
                        <div class="grid grid-cols-[62px_1fr] gap-12.5 border-b border-gray-200 py-5">
                            <h5 class="text-sm text-[#B9B9B9]! ">Phone</h5>
                            <p>+63 93238512313</p>
                        </div>
                        <div class="grid grid-cols-[62px_1fr] gap-12.5 border-b border-gray-200 py-5">
                            <h5 class="text-sm text-[#B9B9B9]! ">Location</h5>
                            <p>Philippines Laguna</p>
                        </div>
                    </div>
                    <h5 class="text-sm text-[#B9B9B9]! mt-5">reply within 1 business day</h5>
                </div>


                <!-- Right -->
                <div class="w-full bg-[#FAFAF7] border border-[#D5D5D5] p-7.5 lg:p-10 rounded-sm">
                    <h3 class="text-3xl">Let's Discuss Your Project</h3>
                    <div class="contact-form flex flex-col gap-5">
                        <div class="mt-7.5 grid grid-cols-1 lg:grid-cols-2 gap-5">
                            <div class="w-full">
                                <label
                                    for="fullname"
                                    class="block mb-2 text-xs font-medium uppercase text-[#AEAEAE]"
                                >
                                    Fullname
                                    <span class="text-[#186534]">*</span>
                                </label>

                                <input
                                    id="fullname"
                                    type="text"
                                    placeholder="Enter your fullname"
                                    class="
                                        w-full
                                        h-12
                                        px-4
                                        rounded
                                        border
                                        border-[#B9B9B9]
                                        bg-transparent
                                        placeholder:text-[#B9B9B9]
                                        outline-none
                                        focus:border-[#186534]
                                        transition-colors
                                    "
                                />
                            </div>
                            <div class="w-full">
                                <label
                                    for="email"
                                    class="block mb-2 text-xs font-medium uppercase text-[#AEAEAE]"
                                >
                                    Email
                                    <span class="text-[#186534]">*</span>
                                </label>

                                <input
                                    id="email"
                                    type="text"
                                    placeholder="Enter your email"
                                    class="
                                        w-full
                                        h-12
                                        px-4
                                        rounded
                                        border
                                        border-[#B9B9B9]
                                        bg-transparent
                                        placeholder:text-[#B9B9B9]
                                        outline-none
                                        focus:border-[#186534]
                                        transition-colors
                                    "
                                />
                            </div>
                        </div>

                        <div class="w-full organization">
                            <label
                                for="organization"
                                class="block mb-2 text-xs font-medium uppercase text-[#AEAEAE]"
                            >
                                Organization
                                <span class="text-[#186534]">*</span>
                            </label>

                            <input
                                id="organization"
                                type="text"
                                placeholder="Enter your organization"
                                class="
                                    w-full
                                    h-12
                                    px-4
                                    rounded
                                    border
                                    border-[#B9B9B9]
                                    bg-transparent
                                    placeholder:text-[#B9B9B9]
                                    outline-none
                                    focus:border-[#186534]
                                    transition-colors
                                "
                            />
                        </div>
                        
                        <div class="w-full project-type">
                            <label
                                for="project-type"
                                class="block mb-2 text-xs font-medium uppercase text-[#AEAEAE]"
                            >
                                Project Type
                                <span class="text-[#186534]">*</span>
                            </label>

                            <input
                                id="project-type"
                                type="text"
                                placeholder="Tell us what you need..."
                                class="
                                    w-full
                                    h-12
                                    px-4
                                    rounded
                                    border
                                    border-[#B9B9B9]
                                    bg-transparent
                                    placeholder:text-[#B9B9B9]
                                    outline-none
                                    focus:border-[#186534]
                                    transition-colors
                                "
                            />
                        </div>

                        <div class="w-full project-details">
                            <label
                                for="project-details"
                                class="block mb-2 text-xs font-medium uppercase text-[#AEAEAE]"
                            >
                                Project Details
                                <span class="text-[#186534]">*</span>
                            </label>

                            <textarea
                                id="project-details"
                                placeholder="Explain your project..."
                                class="
                                    w-full
                                    h-30
                                    px-3
                                    py-3
                                    rounded-[3px]
                                    border
                                    border-[#B9B9B9]
                                    bg-transparent
                                    text-sm
                                    placeholder:text-[#B9B9B9]
                                    outline-none
                                    resize-none
                                    focus:border-[#186534]
                                    transition-colors
                                "
                            ></textarea>
                        </div>

                        <BaseButton 
                            variant="primary" 
                            size="md"
                            @click="goToPreviousTab"
                        >
                            Send Inquiry
                        </BaseButton>
                    </div>
                </div>
            </div>
        </AppContainer>
    </section>
</template>