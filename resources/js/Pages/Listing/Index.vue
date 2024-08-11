<template>
    <div v-for="listing in listings" :key="listing.id">
        <div>
            <Link :href="`/listing/${listing.id}`">
            <ListingAddress :listing="listing" />
            </Link>
        </div>
        <div>
            <Link :href="`/listing/${listing.id}/edit`">Edit</Link>
        </div>
        <div>
            <Link :href="`/listing/${listing.id}`" method="DELETE">Delete</Link>
        </div>
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
