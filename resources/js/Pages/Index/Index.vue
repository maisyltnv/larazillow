<template>
    <div class="text-red-500">Hello!</div>

    <div>
        Them messageis {{ message }}
    </div>
</template>


<script setup>
defineProps(
    {
        message: String
    }
)
</script>
