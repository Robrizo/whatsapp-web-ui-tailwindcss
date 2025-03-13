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
import { onMounted } from 'vue';
import { initFlowbite } from 'flowbite';

onMounted(() => {
    initFlowbite();

    const themeToggleDarkIcon = document.getElementById('theme-toggle-dark-icon');
    const themeToggleLightIcon = document.getElementById('theme-toggle-light-icon');
    const themeToggleBtn = document.getElementById('theme-toggle');

    // Change the icons inside the button based on previous settings
    if (localStorage.getItem('color-theme') === 'dark' || (!('color-theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
        themeToggleLightIcon.classList.remove('hidden');
    } else {
        themeToggleDarkIcon.classList.remove('hidden');
    }

    themeToggleBtn.addEventListener('click', function () {
        // toggle icons inside button
        themeToggleDarkIcon.classList.toggle('hidden');
        themeToggleLightIcon.classList.toggle('hidden');

        // if set via local storage previously
        if (localStorage.getItem('color-theme')) {
            if (localStorage.getItem('color-theme') === 'light') {
                document.documentElement.classList.add('dark');
                localStorage.setItem('color-theme', 'dark');
            } else {
                document.documentElement.classList.remove('dark');
                localStorage.setItem('color-theme', 'light');
            }
        } else {
            // if NOT set via local storage previously
            if (document.documentElement.classList.contains('dark')) {
                document.documentElement.classList.remove('dark');
                localStorage.setItem('color-theme', 'light');
            } else {
                document.documentElement.classList.add('dark');
                localStorage.setItem('color-theme', 'dark');
            }
        }
    });
});
</script>