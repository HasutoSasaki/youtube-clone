<script setup>
import { Head, Link } from '@inertiajs/vue3';
import NavLayout from '@/Layouts/NavLayout.vue'
// defineProps({
//     canLogin: {
//         type: Boolean,
//     },
// });
</script>

<template>
    <Head title="Youtube" />
    <NavLayout>
        <div class="min-w-full">
            <thead class="border-b">
                <tr class="text-white">
                    <th scope="col" class="text-sm font-medium px-6 py-4 text-left">Videos</th>
                    <th scope="col" class="text-sm font-medium px-6 py-4 text-left">Options</th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-b flex justify-between">
                    <td class="px-6 py-4 w-7/12 text-sm font-medium text-gray-900">
                        <video width="320" src="/videos/seoul.mp4" type="video/mp4" controls></video>
                    </td>
                    <td class="px-6 py-4 w-5/12 text-sm font-medium text-gray-900 relative">
                        <div class="text-white font-extrabold mb-4 ">This is a title</div>
                        <div class="w-full">
                            <button class="
                            text-white
                            absolute
                            bottom-4
                            right-4
                            text-xs
                            bg-red-600
                            hover:bg-red-700
                            font-bold
                            py-1
                            px-1
                            float-right
                            rounded
                            cursor-pointer
                            ">
                                Delete</button>
                        </div>
                    </td>
                </tr>
            </tbody>
        </div>
    </NavLayout>
</template>
