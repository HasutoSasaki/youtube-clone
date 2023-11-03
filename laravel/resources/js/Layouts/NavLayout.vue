<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';

</script>

<template>
    <div class="bg-red-400">
        <div id="TopNav" class="w-[100%]"></div>
        <div id="SideNav"></div>
        <div id="SideNavOverlay"></div>

        <slot />
    </div>
</template>
