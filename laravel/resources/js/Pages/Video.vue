<script setup>
import { Head, Link } from '@inertiajs/vue3';
import NavLayout from '@/Layouts/NavLayout.vue'
import CheckCircle from 'vue-material-design-icons/CheckCircle.vue';
import ThumbUpOutline from 'vue-material-design-icons/ThumbUpOutline.vue';
import ThumbDownOutline from 'vue-material-design-icons/ThumbDownOutline.vue'
// defineProps({
//     canLogin: {
//         type: Boolean,
//     },
// });
</script>

<template>
    <Head title="Youtube" />
    <NavLayout>
        <div class="xl:flex">
            <div class="p-3">
                <video src="/videos/seoul.mp4" controls autoplay></video>
                <div class="text-white text-2xl font-extrabold mt-4">A cool video </div>
                <div class="flex items-center mb-4">
                    <img class="rounded-full m-1.5 mt-2 flex items-baseline w-8 h-8"
                        :src="`https://picsum.photos/id/${(Math.random() * 100).toFixed(0)}/100` || ''" alt="">
                    <div class="pl-2 mt-1">
                        <p class="text-white text-lg font-extrabold flex  items-center ">
                            John Weeks Dev
                            <CheckCircle fillColor="#888888" :size="17" />
                        </p>
                        <div class="text-sm  text-gray-400 font-extrabold">1k views - 3 days ago</div>
                    </div>
                </div>
                <div class="bg-[#3F3F3F] rounded-lg w-full p-3 text-white">
                    <div class="text-white text-lg font-extrabold">1k views - 3 days ago</div>
                    <div class="text-sm font-extrabold mb-6">
                        Lorem ipsum dolor sit amet consectetur adipiscing elit.
                    </div>
                    <div class="text-sm font-extrabold">
                        Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the
                        industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type
                        and scrambled it to make a type specimen book.
                    </div>
                </div>

                <div class="mt-6">
                    <div class="text-white text-lg font-extrabold">12 Comments</div>
                    <div class="flex items-flex mb-4 mt-2">
                        <img class="rounded-full mt-2 w-12 h-12"
                            :src="`https://picsum.photos/id/${(Math.random() * 100).toFixed(0)}/100` || ''" alt="">
                        <div class="pl-6 mt-1">
                            <div class="text-white font-extrabold flex items-baseline">
                                <div>Alex Smith</div>
                                <div class="text-gray-400 pl-3">
                                    6 days ago
                                </div>
                            </div>
                            <div class="text-gray-200 text-sm font-semibold">
                                Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum
                                has been the industry's standard dummy text ever since the 1500s, when an unknown
                                printer took a galley of type and scrambled it to make a type specimen book.
                            </div>
                            <div class="mt-4 flex items-center">
                                <ThumbUpOutline fillColor="#FFFFFF" :size="20" class="pr-2" />
                                <div class="text-gray-400 text-sm font-extrabold pr-10">
                                    {{ (Math.random() * 100).toFixed(0) }}
                                </div>
                                <ThumbDownOutline fillColor="#FFFFFF" :size="20" />
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </NavLayout>
</template>

<style>
.bg-dots-darker {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}

@media (prefers-color-scheme: dark) {
    .dark\:bg-dots-lighter {
        background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
    }
}
</style>
