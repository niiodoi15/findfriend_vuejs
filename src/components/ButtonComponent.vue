<script setup>
    defineProps(['buttontext']);
    defineEmits(['addone'])
</script>

<template>
    <button class="btn">{{ buttontext }}</button>
    <!-- <button class="btn" @click="emit('addone')">Increase</button> -->
</template>

<style>
    .btn{
        padding: 12px 32px;
        gap: 10px;
        border-radius: 40px;
        background: #FFF;
        border: none;
    }
</style>