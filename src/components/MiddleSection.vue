<template>
    <!-- middle section -->
    <div
        class="bg-white border-x-2 border-gray-200 dark:border-[#26353d] dark:bg-[#0f1a1f] min-w-[360px] w-[480px]  h-full flex flex-col">
        <!-- header section -->
        <div class="px-4 py-2">
            <!-- header  -->
            <div class="flex items-center justify-between">
                <div class="text-2xl text-[#111b21] dark:text-gray-300 font-bold">
                    <h1>Chats</h1>
                </div>
                <div class="flex items-center space-x-4">
                    <button
                        class="relative group h-10 w-10 flex items-center justify-center rounded-full cursor-pointer">
                        <NewChatIcon />
                        <span
                            class="bg-white text-xs p-1 border dark:border-none absolute -bottom-5 -right-10 z-10 whitespace-nowrap opacity-0 invisible transition-opacity group-hover:duration-300 group-hover:delay-300  group-hover:opacity-100 group-hover:visible">
                            New chat
                        </span>
                    </button>
                    <button
                        class="relative group h-10 w-10 flex items-center justify-center rounded-full cursor-pointer">
                        <MenuIcon />
                        <span
                            class="bg-white text-xs p-1 border dark:border-none absolute -bottom-4 -right-6 z-10 whitespace-nowrap opacity-0 invisible transition-opacity group-hover:duration-300 group-hover:delay-300  group-hover:opacity-100 group-hover:visible">
                            Menu
                        </span>
                    </button>

                </div>
            </div>

            <!-- search -->
            <div class="relative w-full flex items-center mt-4">
                <input type="search" placeholder="Search"
                    class="w-full py-1.5 pl-16 pr-4 bg-[#f0f2f5] dark:bg-[#222e35] text-[#54656f] dark:text-gray-300 font-light rounded-lg placeholder:text-gray-400 border-none focus:ring-0 focus:outline-none">
                <SearchIcon class="absolute left-4" />
            </div>

            <!-- filter -->
            <div class="w-full flex space-x-2 mt-2">
                <div
                    class="bg-[#e7fce3] dark:bg-[#0a332c] text-[#008069] dark:text-[#00a884] text-sm font-light rounded-full px-4 py-1 cursor-pointer">
                    All
                </div>
                <button
                    class="bg-[#f0f2f5] dark:bg-[#222e35] text-[#54656f] dark:text-gray-400 text-sm font-light rounded-full px-4 py-1 hover:bg-[#e9edef] dark:hover:bg-[#26353d] cursor-pointer">
                    Unread</button>
                <button
                    class="bg-[#f0f2f5] dark:bg-[#222e35] text-[#54656f] dark:text-gray-400 text-sm font-light rounded-full px-4 py-1 hover:bg-[#e9edef] dark:hover:bg-[#26353d] cursor-pointer">Favorites</button>
                <button
                    class="bg-[#f0f2f5] dark:bg-[#222e35] text-[#54656f] dark:text-gray-400 text-sm font-light rounded-full px-4 py-1 hover:bg-[#e9edef] dark:hover:bg-[#26353d] cursor-pointer">Groups</button>
            </div>
        </div>
        <!-- end header section -->

        <!-- chats section -->
        <div
            class="relative w-full mx-auto h-full flex-1 overflow-y-auto scrollbar-thin scrollbar-thumb-gray-300 scrollbar-track-white dark:scrollbar-track-[#0f1a1f] dark:scrollbar-thumb-[#222e35]">
            <!-- chart card 1-->
            <div
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/rjc.jpg" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21]  dark:text-gray-300 text-lg">Robert</h3>
                        <span class="text-[#667781] dark:text-gray-400 text-xs">02:00 pm</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <BlueTickIcon />
                            <span class="text-[#667781] dark:text-gray-400 text-sm font-light line-clamp-1">😂😂 mfana
                                wachibwana
                                iwe eti🚮🚮. Malawi wavuta uyu</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 1 -->
            <!-- chart card 2-->
            <div
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/manu.png" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21] dark:text-gray-300 text-lg font-bold">Manchester United Fans⚽</h3>
                        <span class="text-[#1fa855] dark:text-[#00a884] text-xs font-bold">05:48 pm</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <span class="text-[#21c063] text-sm font-bold line-clamp-1">~Top Fun is
                                typing...</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <span
                                class="bg-[#25d366] dark:bg-[#00a884] text-white dark:text-[#111b21] text-sm h-5 min-w-[20px] px-1 flex items-center justify-center rounded-full">
                                102
                            </span>
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 2 -->
            <!-- chart card 3-->
            <div
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/pic.jpg" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21] dark:text-gray-300 text-lg">Ankolo</h3>
                        <span class="text-[#667781] dark:text-gray-400 text-xs">Yesterday</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <TickIcon />
                            <span class="text-[#667781] dark:text-gray-400 text-sm font-light line-clamp-1">Arsenal is
                                useless</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 3 -->
            <!-- chart card 4-->
            <div
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/profile.jpg" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21] dark:text-gray-300 text-lg">Mary Phiri</h3>
                        <span class="text-[#667781] dark:text-gray-400 text-xs">07:02 pm</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <BlueTickIcon />
                            <MicIcon />
                            <span class="text-[#667781] dark:text-gray-400 text-sm font-light line-clamp-1">0:36</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 4 -->
            <!-- chart card 5-->
            <div
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/mary.png" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21] dark:text-gray-300 text-lg font-bold">Programmer 01</h3>
                        <span class="text-[#1fa855] dark:text-[#00a884] text-xs font-bold">10:32 am</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <span class="text-[#3b4a54] dark:text-gray-400 text-sm font-bold line-clamp-1">Thanks
                                boss</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <span
                                class="bg-[#25d366] dark:bg-[#00a884] text-white dark:text-[#111b21] text-sm h-5 min-w-[20px] px-1 flex items-center justify-center rounded-full">
                                3
                            </span>
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 5 -->
            <!-- chart card 6-->
            <div v-for="i in 4"
                class="group w-full flex items-center space-x-4 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#26353d] dark:hover:outline-2 dark:hover:outline-[#26353d] pl-4">
                <div class="relative">
                    <div class="w-12 h-12">
                        <img src="@/assets/images/movie4.jpg" alt=""
                            class="w-full h-full object-cover object-center rounded-full">
                    </div>
                </div>
                <div class="w-full flex flex-col border-t border-gray-200 dark:border-[#26353d] py-3">
                    <div class="flex items-center justify-between space-x-2 pr-4">
                        <h3 class="text-[#111b21] dark:text-gray-300 text-lg">Macheza Promax😂😂</h3>
                        <span class="text-[#667781] dark:text-gray-400 text-xs">Thursday</span>
                    </div>
                    <div class="flex items-center justify-between pr-4">
                        <div class="flex items-center space-x-1">
                            <span class="text-[#667781] dark:text-gray-400 text-sm font-light line-clamp-1">~Top Fun:
                                Mkona unachotsedwa
                                mano iwe</span>
                        </div>
                        <div class="relative group flex items-center justify-center space-x-2 pl-2">
                            <div class="relative group-hover:w-5">
                                <AngleDownIcon
                                    class="absolute inset-y-0 right-0 flex items-center justify-center transform translate-x-4 opacity-0 transition-all group-hover:translate-x-0 group-hover:opacity-100" />
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- end chart card 6 -->
            <div class="border-t border-gray-200 dark:border-[#26353d] py-4 mt-4 mx-4">
                <div class="flex justify-center space-x-2">
                    <LockIcon />
                    <p class="text-xs text-[#667781] dark:text-gray-400">Your personal messages are
                        <a href="#" class="text-[#21c063] hover:underline cursor-pointer">
                            end-to-end encrypted
                        </a>
                    </p>
                </div>
            </div>
        </div>
    </div>
    <!-- end middle section -->
</template>

<script setup>
import SearchIcon from '@/components/icons/SearchIcon.vue'
import LockIcon from '@/components/icons/LockIcon.vue'
import NewChatIcon from '@/components/icons/NewChatIcon.vue'
import MenuIcon from '@/components/icons/MenuIcon.vue'
import AngleDownIcon from '@/components/icons/AngleDownIcon.vue'
import TickIcon from '@/components/icons/TickIcon.vue'
import BlueTickIcon from '@/components/icons/BlueTickIcon.vue'
import MicIcon from '@/components/icons/MicIcon.vue'
</script>