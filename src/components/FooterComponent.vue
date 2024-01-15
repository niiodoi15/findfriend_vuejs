<script setup>

</script>

<template>
    <div class="footer">
        <div class="footernav">
            <div class="footerlog">
                <img src="../assets/footerlogo.png" class="footerimage">
                <p class="footlogt">Findtrend</p>
            </div>
            <div class="footerlinks">
                <a href="" class="item-footer">Privacy Policy</a>
                <a href="" class="item-footer">Terms and Conditions</a>
                <a href="" class="item-footer">Contact Us</a>
                <a href="" class="item-footer">Careers</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer{
    padding: 10%;
}
.footernav{
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: center;
}
.footerimage{
    width: 40px;
    height: 40px;
}
.footerlog{
    display: flex;
    gap: 20px;
    align-items: center;
}
.footerlinks{
    display: flex;
    flex-direction: column;
    gap: 30px;
}
    .footlogt{
        color: #000;
        text-align: center;
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 24px;
    }
    .item-footer{
        color: #000;
        text-align: center;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 18px;
        text-decoration: none;
    }
    @media (min-width: 732px){
        .footernav{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }
    .footerlinks{
        display: flex;
        flex-direction: row;
        gap: 30px;
    }
    .footer{
        padding: 3%;
    }
    }
</style>