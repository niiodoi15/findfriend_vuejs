<script setup>
import ButtonComponent from './ButtonComponent.vue';


</script>

<template>
    <div class="join">
        <h1 class="jointext">Join us on email for</h1>
        <div class="joinpara">more trending topics</div>
        <ButtonComponent class="joinbtn" buttontext="Join Now"/>
    </div>
</template>

<style scoped>
.join{
    padding: 10%;
    background: #A8FF35;
    display: flex;
    justify-content: center;
    flex-direction: column;
    /* gap: 10px; */
}
    .jointext{
        color: #000;
        text-align: center;
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
    }
    .joinpara{
        color: #87D322;
        text-align: center;
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
        margin-bottom: 20px;
    }
    .joinbtn{
        margin: 0 auto;
        background-color: #000;
        color: #fff;
    }
    @media (min-width: 678px){
        .jointext{
        color: #000;
        text-align: center;
        font-size: 72px;
        font-style: normal;
        font-weight: 900;
        line-height: 80.64px;
    }
    .joinpara{
        color: #87D322;
        text-align: center;
        font-size: 72px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
        margin-bottom: 20px;
    }
    }
</style>