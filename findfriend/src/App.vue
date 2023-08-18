<script setup>
  import HeaderComponent from './components/HeaderComponent.vue';
import OpentabComponent from './components/OpentabComponent.vue';

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
</template>

<style scoped>
.textsection{
  padding: 10%;
}
.trend{
  color: #000;
  font-family: Effra;
  font-size: 36px;
  font-style: normal;
  font-weight: 900;
  line-height: normal;
}
.trend span{
  color: #ADADAD;
  font-family: Effra;
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
