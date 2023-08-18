<script setup>
    import ButtonComponent from './ButtonComponent.vue';
    import HeroCardComponent from './HeroCardComponent.vue';


</script>

<template>
    <header>
        <div class="navbar">
          <div class="logodiv">
            <img src="../assets/logofriend.png" alt="" class="logo">
            <p class="logotext">Findtrend</p>
          </div>
          <div class="links">
            <a href="" class="link-item">About</a>
            <a href="" class="link-item">How it works</a>
            <a href="" class="link-item">Prcing</a>
            <a href="" class="link-item">Solution</a>
            <a href="" class="link-item">Features</a>
          </div>
          <div class="navbuttons">
            <a href="">Login</a>
            <ButtonComponent buttontext="Register"/>
          </div>
          <div class="humberger">
            <div></div>
            <div></div>
          </div>
        </div>
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
            <!-- require('../assets/twitter.png') -->
            <HeroCardComponent cardimages="@/assets/twitter.png"  cardtext="Cryptopunk - Search"/>
            <HeroCardComponent class="carditem1" cardimages="../assets/pinterest" cardtext="Popular Design - Search"/>
            <HeroCardComponent class="carditem2" cardimages="../assets/twitter.png" cardtext="Product Design - Search"/>
            <HeroCardComponent class="carditem3" cardimages="../assets/twitter.png" cardtext="Elon Musk - Search"/>
        </div>
      </header>
</template>

<style scoped>
    header{
        background-color: black;
        padding: 0 3rem 7rem 3rem;
        display: flex;
        flex-direction: column;
        gap: 60px;
    }
    .navbar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0.5rem;
    }
    .navbuttons, .links, .logotext{
        display: none;
    }
    .humberger div{
        width: 30px;
        height: 5px;
        margin-bottom: 5px;
        background-color: #fff;
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
        font-family: Effra;
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40.32px;
    }
    .paragraph{
        color: #8B8B8B;
        text-align: center;
        font-family: Effra;
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
        justify-content: center;
        align-items: center;
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

    @media (min-width: 732px){
        .logotext{
        color: #FFF;
        text-align: center;
        font-family: Inter;
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 24px;
        }
        .navbuttons{
            display: flex;
            gap: 0.7rem;
            align-items: center;
        }
        .navbuttons a{
            color: #FFF;
            text-align: center;
            font-family: Effra;
            font-size: 18px;
            font-style: normal;
            font-weight: 400;
            line-height: 18px;
            text-decoration: none;
        }
        .links{
            display: flex;
            gap: 2rem;
            align-items: center;
        }
        .link-item{
            color: #FFF;
            text-align: center;
            font-family: Effra;
            font-size: 18px;
            font-style: normal;
            font-weight: 400;
            line-height: 100%; /* 18px */
            text-decoration: none;
        }
        .humberger{
            display: none;
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
            flex-direction: row;
            position: relative;
            justify-content: left;
        }
        .carditem1{
            position: absolute;
            left: 25%;
            top: 40%;
            z-index: 4;
        }
        .carditem2{
            position: absolute;
            left: 50%;
            z-index: 3;
        }
        .carditem3{
            position: absolute;
            left: 70%;
            top: 40%;
            z-index: 2;
        }
        
    }
</style>