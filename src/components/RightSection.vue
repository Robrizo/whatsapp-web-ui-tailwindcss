<template>
    <div class="relative min-w-[360px] mx-auto h-full p-6">
        <div class="w-full h-full flex flex-col space-y-8 items-center justify-center">
            <div class="w-[300px] flex items-center justify-center">
                <img src="@/assets/images/whatsapp_web.png" alt="" class="w-full h-full object-contain object-center">
            </div>

            <div class="w-full space-y-6 flex flex-col items-center">
                <h3 class="text-center text-gray-300 text-4xl font-extralight">Download WhatsApp for Windows</h3>
                <p class="max-w-lg text-center text-sm font-light text-gray-400">
                    Make calls, share your screen and get a faster experience when you download the Windows app.
                </p>
                <button
                    class="bg-[#00a884] text-[#111b21] text-sm font-medium tracking-wide px-6 py-2.5 rounded-full hover:bg-[#06cf9c] cursor-pointer">
                    Download
                </button>
            </div>

            <div class="absolute bottom-10 flex items-center space-x-2">
                <LockIcon />
                <p class="text-sm font-extralight text-gray-400">Your personal messages are end-to-end encrypted</p>
            </div>
        </div>
    </div>
</template>

<script setup>
import LockIcon from '@/components/icons/LockIcon.vue';
</script>