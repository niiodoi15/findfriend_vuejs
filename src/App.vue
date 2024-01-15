<script setup>
  import DealComponent from './components/DealComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import JoinComponent from './components/JoinComponent.vue';
  import OpentabComponent from './components/OpentabComponent.vue';
import SociacardComponent from './components/SociacardComponent.vue';
  import StartupComponent from './components/StartupComponent.vue';
import FooterComponent from './components/footerComponent.vue';
  
  
</script>

<template>  
  <HeaderComponent />
  <OpentabComponent />
  <div class="textsection">
    <h2 class="trend">
      Findtrend helps you to increase your
      productivity and reduce your computer's
      memory load,<span> an application that can 
      fulfill your daily browsing needs.</span>
    </h2>
  </div>
  <StartupComponent />
  <SociacardComponent />
  <DealComponent />
  <JoinComponent />
  <FooterComponent />
</template>

<style scoped>

  @import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

.textsection{
  padding: 10%;
}
.trend{
  color: #000;
  font-family: 'Ubuntu';
  font-size: 36px;
  font-style: normal;
  font-weight: 900;
  line-height: normal;
}
.trend span{
  color: #ADADAD;
  font-family: 'Ubuntu';
  font-size: 36px;
  font-style: normal;
  font-weight: 900;
  line-height: normal; 
}
@media (min-width: 734px){
  .trend{
  font-size: 64px;
  font-weight: 700;
}
.trend span{
  color: #ADADAD;
  font-size: 64px;
  font-weight: 700;
}
}
</style>
