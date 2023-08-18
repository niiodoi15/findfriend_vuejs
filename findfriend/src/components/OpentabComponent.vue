<script setup>

</script>

<template>
    <div class="opentab">
        <h1 class="opentext">Open new tabs is sh*t </h1>
        <div class="opencenter">
            <p><img class="firstimg" src="../assets/Group 427321661.png"></p>
            <div class="logocenter">
                <img class="centerimg" src="../assets/Grouplogo.png">
            </div>
           <p> <img class="secondimg" src="../assets/Group 427321658.png"></p>
        </div>
        <p class="openpara">A solution for your browser tabs and don’t make your device get slower over time. Get ease and faster to discover a trend with just one tab.</p>
    </div>
</template>

<style scoped>
.opentab{
    background-color: #A8FF35;
    display: flex;
    flex-direction: column;
    gap: 70px;
    padding: 60px 0;
}
.opencenter{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    position: relative;
    height: 200px;
}
.firstimg{
    position: absolute;
    bottom: 0;
}
.secondimg{
    position: absolute;
    top: 0;
    right: 15%;
}
    .opentext{
        color: #000;
        text-align: center;
        font-family: Effra;
        font-size: 36px;
        font-weight: 700;
        line-height: 40.32px;
    }
    .logocenter{
        padding: 24px;
        background-color: #F5F5F5;
        max-width: 339px;
        height: 118px;
        border-radius: 14px;
    }
    .openpara{
        color: #000;
        text-align: center;
        align-self: center;
        font-family: Effra;
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 21px;
        max-width: 286px;
    }

    @media (min-width: 732px){
        
        .opentab{
            padding: 140px 0;
        }
        .logocenter{
            padding: 24px;
            background-color: #F5F5F5;
            max-width: 502px;
            height: 202px;
            border-radius: 16px;
            display: flex;
            justify-content: center;
            align-items: center;

        }   
        .centerimg{
            width: 341.226px;
            height: 82px;
            flex-shrink: 0;
        }
    .opentext{
        font-size: 72px;
    }
    .openpara{
        font-size: 18px;
        max-width: 600px;
    }
    .firstimg{
    position: static;
}
.secondimg{
    position: static;
}
}
</style>