<script setup>
    defineProps(['buttontext']);
</script>

<template>
    <button class="btn">{{ buttontext }}</button>
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