<template>
    <div class="relative w-screen h-screen bg-gray-300 dark:bg-[#222e35]">
        <div class="absolute top-0 w-full h-32 bg-[#00a884]"></div>
        <div class="relative z-20 dark:bg-[#292725] w-full h-full mx-auto 2xl:p-5">
            <div class="flex mx-auto h-full bg-[#f0f2f5] dark:bg-[#222e35]">
                <LeftSection />
                <MiddleSection />
                <RightSection />
            </div>
        </div>
    </div>
</template>

<script setup>
import LeftSection from '@/components/LeftSection.vue'
import RightSection from '@/components/RightSection.vue'
import MiddleSection from '@/components/MiddleSection.vue';
</script>