<script setup>
defineProps(["mediaimages"])
</script>

<template>
    <div class="cardcontainer">
        <img :src="mediaimages" alt="logo">
    </div>
</template>

<style scoped>
.cardcontainer {
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 8px;
    padding: 25px;
    background: #FFF;
}

.cardcontainer img {
    max-height: 30px;
    height: 100%;
    /* width: 80px; */
}
</style>