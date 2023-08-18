<script setup>
    import { defineProps } from 'vue';
    defineProps(['cardimages', 'cardtext']);
</script>

<template>
    <div class="card-item">
        <div class="card-text">
            <img :src="cardimages" alt="">
            <p class="cardp">{{ cardtext }}</p>
        </div>
        <p class="cancel"><img src="../assets/cancels.png" alt=""></p>
    </div>
</template>

<style scoped>
.card-item{
    width: 341.226px;
    height: 82px;
    transform: rotate(-4deg);
    background: rgba(24, 24, 24, 1);
    position: relative;
    display: flex;
    align-items: center;
    padding: 0 41px;
    z-index: 5;
    
}
    .card-text{
        display: flex;
        gap: 10px;
        align-items: center;
        justify-content: center;
    }
    .cardp{
        color: #FFF;
        text-align: center;
        font-family: Roboto;
        font-size: 20.445px;
    }
    .cancel{
        position: absolute;
        right: 0;
        padding: 10px 20px;
        background: linear-gradient(270deg, #181818 53.65%, rgba(24, 24, 24, 0.80) 100%);
    }
</style>