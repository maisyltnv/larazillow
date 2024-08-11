<template>
    <div v-for="listing in listings" :key="listing.id">
        <Link :href="`/listing/${listing.id}`">
        <ListingAddress :listing="listing"/>
        </Link>
    </div>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
import { defineProps } from 'vue';
import ListingAddress from "../../Components/ListingAddress.vue";

// Define props for the component
const props = defineProps({
    listings: Array
});
</script>
