<template>
   <Link href="/listing">Main Page</Link>
   <Link href="/listing/create" >Show Page</Link>

   <div v-if="flashSuccess" class="success">{{flashSuccess}}</div>

    
   <slot>Default</slot>
</template>

<script setup>
import {computed} from 'vue';
import { Link ,usePage} from '@inertiajs/vue3';

//flash success
const page = usePage()
const flashSuccess = computed(() => page.props.flash.success)

</script>


<style scoped>
.success {
   background-color: green;
   color:white
}
</style>