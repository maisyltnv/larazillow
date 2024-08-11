<template>
    <MainLayout>
        <div class="text-red-500">Hello!</div>

        <div>
            Them messageis {{ message }}
        </div>
    </MainLayout>

</template>




<script setup>

import { Link } from '@inertiajs/vue3';
import MainLayout from '../../Layouts/MainLayout.vue';
defineProps(
    {
        message: String
    }
)

</script>