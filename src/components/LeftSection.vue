<template>
    <div class="flex h-full w-16 border-r-2 border-[#26353d] flex-col items-center justify-between px-6 py-3">
        <!-- top content -->
        <div class="space-y-4">
            <IconButton :icon="ChatIcon" :count="31" tooltip="Chats" />
            <IconButton :icon="StatusIcon" tooltip="Status" />
            <IconButton :icon="ChannelsIcon" tooltip="Channels" />
            <IconButton :icon="CommunityIcon" tooltip="Communities" />
            <IconButton :icon="meta_image" tooltip="Meta AI" />
        </div>

        <!-- bottom content -->
        <div class="space-y-4">
            <IconButton :icon="GearIcon" tooltip="Settings" />
            <IconButton :icon="profile_image" tooltip="Profile" height="h-8" width="w-8"/>
        </div>
    </div>
</template>

<script setup>
import IconButton from '@/components/IconButton.vue'
import ChatIcon from '@/components/icons/ChatIcon.vue'
import StatusIcon from '@/components/icons/StatusIcon.vue'
import ChannelsIcon from '@/components/icons/ChannelsIcon.vue'
import CommunityIcon from '@/components/icons/CommunityIcon.vue'
import GearIcon from '@/components/icons/GearIcon.vue'

import meta_image from '@/assets/images/meta.png'
import profile_image from '@/assets/images/rjc.jpg'
</script>