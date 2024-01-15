<script setup>
import MediaComponent from './Mediacomponent.vue';
import twitter from '../assets/twitter.png';
import pinterest from '../assets/pinterest.png';
import facebook from '../assets/facebook.png';
import basketball from '../assets/basketball.png';
import ButtonComponent from './ButtonComponent.vue';

</script>

<template>
    <div class="sponsorcontainer">
        <h1 class="startuptext">All platform connect to Findtrend</h1>
        <div class="container">
            <div class="socialcards1">
                <MediaComponent :mediaimages="pinterest" />
                <MediaComponent class="twitterimg" :mediaimages="twitter" />
                <MediaComponent :mediaimages="facebook" />
                <MediaComponent :mediaimages="basketball" />
                <MediaComponent class="lost" :mediaimages="pinterest" />
                <MediaComponent class="lost" :mediaimages="twitter" />
                <MediaComponent class="lost" :mediaimages="facebook" />
                <MediaComponent class="lost" :mediaimages="basketball" />
                
            </div>
        </div>
        <div class="textimage">
            <img src="../assets/tweets1.png" alt="">
            <img src="../assets/tweets2.png" alt="">
            <img src="../assets/tweets3.png" alt="">
        </div>
        <div class="btndiv">
            <ButtonComponent class="blackbtn" buttontext="View More Trend"/>
        </div>
    </div>
</template>

<style scoped>

.sponsorcontainer {
    padding: 10%;
    display: flex;
    flex-direction: column;
    gap: 32px;
    background-color: #FAFAFA;

}

.startuptext {
    color: #000;
    text-align: center;
    font-family: 'Ubuntu';
    font-size: 32px;
    font-weight: 900;
}
.container{
    display: flex;
}
.socialcards1 {
    display: flex;
    justify-content: center;
    gap: 10px;
}
.lost{
    display: none;
}
.twitterimg{
    background-color: #A8FF35;
}
.textimage{
    display: flex;
    flex-direction: column;
    gap: 25px;
}
.textimage img{
    max-width: 339px;
    margin: 0 auto;
}
.btndiv{
    text-align: center;
}
.blackbtn{
    background: #000;
    color: #fff;
}
@media (min-width: 678px) {
    .startuptext {
        font-weight: 700;
        font-size: 64px;
    }
    .textimage img{
    max-width: 600px;
    margin: 0 auto;
    }
}</style>