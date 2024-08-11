<template>
   <Link href="/listing">Main Page</Link>
   <Link href="/listing/create">Show Page</Link>

    


   <slot>Default</slot>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
import {ref} from "vue";


</script>
