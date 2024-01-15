<script setup>
    import { defineProps } from 'vue';
    defineProps(['cardimages', 'cardtext']);
</script>

<template>
    <div class="card-item">
        <div class="card-text">
            <img class="sologos" :src="cardimages" alt="thee">
            <p class="cardp">{{ cardtext }}</p>
        </div>
        <p class="cancel"><img src="../assets/cancels.png" alt=""></p>
    </div>
</template>

<style scoped>
.card-item{
    width: 290px;
    /* height: 82px; */
    transform: rotate(-4deg);
    background: rgba(24, 24, 24, 1);
    position: relative;
    display: flex;
    align-items: center;
    padding: 15px 15px;
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
        font-family: 'Ubuntu';
        font-size: 18px;
    }
    .sologos{
        height: 27px;
    }
    .cancel{
        position: absolute;
        right: 0;
        padding: 10px 20px;
        background: linear-gradient(270deg, #181818 53.65%, rgba(24, 24, 24, 0.80) 100%);
    }
</style>