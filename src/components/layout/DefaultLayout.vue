<template>
    <div class="bg-[#292725] w-screen h-screen mx-auto 2xl:p-5">
        <div class="flex mx-auto h-full bg-[#222e35]">
            <LeftSection />
            <MiddleSection />
            <RightSection />
        </div>
    </div>
</template>

<script setup>
import LeftSection from '@/components/LeftSection.vue'
import RightSection from '@/components/RightSection.vue'
import MiddleSection from '@/components/MiddleSection.vue';
</script>