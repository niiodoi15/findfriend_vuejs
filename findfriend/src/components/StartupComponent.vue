<script setup>
import LogoComponent from './LogoComponent.vue';
import microsoft from '../assets/microsoft.png';
import allianz from '../assets/allianz.png';
import upwork from '../assets/upwork.png';
import volvo from '../assets/volvo.png';
import grab from '../assets/grab.png';
import verizon from '../assets/verizon.png';
import coinbase from '../assets/coinbase.png'; 
import expedia from '../assets/expedia.png';
import airtoble from '../assets/airtoble.png';
import magento from '../assets/magento.png';
import carrera from '../assets/carrera.png';
import bonanza from '../assets/bonanza.png';
import wetransfer from '../assets/wetransfer.png';
import suzuki from '../assets/suzuki.png';
import aloglia from '../assets/algolia.png';
import heineken from '../assets/heineken.png';
</script>

<template>
    <div class="sponsorcontainer">
        <h1 class="startuptext">Findtrend make +1000 Startup grow</h1>
        <div class="sponsor">
            <LogoComponent :logoimages="microsoft"/>
            <LogoComponent :logoimages="allianz"/>
            <LogoComponent :logoimages="upwork"/>
            <LogoComponent :logoimages="volvo"/>
            <LogoComponent :logoimages="grab"/>
            <LogoComponent :logoimages="verizon"/>
            <LogoComponent :logoimages="coinbase"/>
            <LogoComponent :logoimages="expedia"/>
            <LogoComponent :logoimages="airtoble"/>
            <LogoComponent :logoimages="magento"/>
            <LogoComponent :logoimages="carrera"/>
            <LogoComponent :logoimages="bonanza"/>
            <LogoComponent :logoimages="wetransfer"/>
            <LogoComponent :logoimages="suzuki"/>
            <LogoComponent :logoimages="aloglia"/>
            <LogoComponent :logoimages="heineken"/>
        </div>
    </div>
</template>

<style scoped>
    .sponsorcontainer{
        padding: 10%;
        display: flex;
        flex-direction: column;
        gap: 32px;
        
    }
    .startuptext{
        color: #000;
        text-align: center;
        font-family: 'Ubuntu';
        font-size: 32px;
        font-weight: 900;
    }
    .sponsor{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-gap: 10px;
    }

    @media (min-width: 678px){
       .startuptext{
            font-weight: 700;
            font-size: 64px;
        } 
        .sponsor{
        grid-template-columns: repeat(4, 1fr);
        }
    }
</style>