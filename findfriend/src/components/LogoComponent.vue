<script setup>
    defineProps(["logoimages"])
</script>

<template>
    <div class="cardcontainer">
        <img :src="logoimages" alt="">
    </div>
</template>

<style scoped>
    .cardcontainer{
        width: 162px;
        height: 74px;
        flex-shrink: 0;
    }
</style>