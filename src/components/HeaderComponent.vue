<script setup>
    import ButtonComponent from './ButtonComponent.vue';
    import HeroCardComponent from './HeroCardComponent.vue';
    import twitter from '../assets/twitter.png';
    import pinterest from '../assets/pinterest.png';
    import facebook from '../assets/facebook.png';
    import basketball from '../assets/basketball.png';
    import NavbarComponent from './NavbarComponent.vue';

</script>

<template>
    <header>
        <NavbarComponent />
        <div class="header-text">
            <h2 class="heading">Minimize your tabs. <br> Find the trends!</h2>
            
            <p class="paragraph">
                Don’t let your computer memories consumes all of those browser tabs. 
                Findtrend  let you gathers all of your favorite website into one place.
            </p>
        </div>
        <div class="herobtn">
            <ButtonComponent class="midbtn" buttontext="Get Started 🔥"/>
            <img class="btn-arrow" src="../assets/img-hero.png" alt="img-ll">
        </div>

        <div class="herocards">
            <HeroCardComponent class="carditem0" :cardimages="twitter"  cardtext="Cryptopunk - Search"/>
            <HeroCardComponent class="carditem1" :cardimages="pinterest" cardtext="Popular Design - Search"/>
            <HeroCardComponent class="carditem2" :cardimages="facebook" cardtext="Product Design - Search"/>
            <HeroCardComponent class="carditem3" :cardimages="basketball" cardtext="Elon Musk - Search"/>
        </div>
      </header>
</template>

<style scoped>
    header{
        background-color: black;
        background-image: url(../assets/Ornament.svg);
        padding: 0 4rem 7rem 4rem;
        display: flex;
        flex-direction: column;
        gap: 60px;
    }
    .midbtn{
        background: #A8FF35;
    }
    .header-text{
        display: flex;
        flex-direction: column;
        gap: 24px;
    }

    .heading{
        color: #FFF;
        text-align: center;
        font-family: 'Ubuntu';
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40.32px;
    }
    .paragraph{
        color: #8B8B8B;
        text-align: center;
        font-family: 'Ubuntu';
        font-size: 14px;
        font-weight: 400;
        line-height: 21px;
        max-width: 286px;
        margin: 0 auto;
    }
    .herobtn{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .btn-arrow{
        display: none;
    }
    .herocards{
        display: flex;
        flex-direction: column;
        /* justify-content: center; */
        align-items: center;
        position: relative;
    }
    .carditem1{
        transform: rotate(2deg);
    }
    .carditem2{
        transform: rotate(-2deg);
    }
    .carditem3{
        transform: rotate(4deg);
    }
    .logodiv{
        display: flex;
        align-items: center;
        gap: 5px;
    }

    @media (min-width: 769px){
        header{
            gap: 100px;
        }
        .heading{
            font-size: 72px;
            line-height: 80.64px ;
        }
        .paragraph{
            font-size: 18px;
            line-height: 27px;
            max-width: 600px;
            margin: 0 auto;
        }
        .btn-arrow{
            display: block;
        }
        .herocards{
            /* flex-direction: row; */
            position: relative;
            /* max-width: 700px; */
            /* justify-content: center; */
            /* align-items: center; */
            padding: 0 10%;
            /* margin: 0 auto; */
            background-color: #A8FF35;
        }
        .carditem0{
            position: absolute;
            left: 5%;
            bottom: 0;
            z-index: 5;
        }
        .carditem1{
            position: absolute;
            left: 25%;
            top: -12px;
            /* bottom: 10%; */
            z-index: 4;
        }
        .carditem2{
            position: absolute;
            right: 25%;
            bottom: 0px;
            z-index: 5;
        }
        .carditem3{
            position: absolute;
            right: 5%;
            /* bottom: 2%; */
            top: -12px;
            z-index: 2;
        }
        
    }
</style>