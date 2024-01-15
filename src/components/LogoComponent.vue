<script setup>
    defineProps(["logoimages"])
</script>

<template>
    <div class="cardcontainer">
        <img :src="logoimages" alt="logo">
    </div>
</template>

<style scoped>
    .cardcontainer{
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 8px;
        padding: 30px;
        background-color: #F5F5F5;
    }
    .cardcontainer img{
        max-height: 50px;
        height: 100%;
        width: 60px;
    }
</style>