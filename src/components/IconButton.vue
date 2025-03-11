<template>
    <div class="relative group">
        <button class="h-10 w-10 flex items-center justify-center rounded-full cursor-pointer"
            :class="{ 'bg-[#434f4f]': icon === 'ChatIcon' }">
            <component :is="icon" v-if="typeof icon === 'object'" />
            <img v-else-if="typeof icon === 'string'" :src="icon" alt="" :class="`${height} ${width} object-cover object-center rounded-full`">
            <div v-if="count"
                class="h-5 w-5 absolute -top-1 -right-1 bg-[#00a884] text-xs tracking-tighter font-medium rounded-full flex items-center justify-center">
                {{ count }}
            </div>
        </button>
        <div
            class="opacity-0 invisible absolute z-10 top-1 left-12 bg-gray-100 text-sm text-gray-700 rounded-full px-4 py-1 whitespace-nowrap transition-opacity group-hover:duration-300 group-hover:delay-300 group-hover:opacity-100 group-hover:visible">
            {{ tooltip }}
        </div>
    </div>
</template>

<script setup>
defineProps({
    icon: {
        type: [String, Object],
        required: true
    },
    count: {
        type: [String, Number],
        default: null
    },
    tooltip: {
        type: String,
        default: ''
    },
    height: {
        type: String,
        default: 'h-5'
    },
    width: {
        type: String,
        default: 'w-5'
    }
});
</script>
