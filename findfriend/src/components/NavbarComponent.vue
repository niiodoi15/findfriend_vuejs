<script setup>
  import ButtonComponent from './ButtonComponent.vue';
</script>

<template>
  <div class="navbar">
    <div href="" class="logodiv">
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
      <a class="link-item" href="">Login</a>
      <ButtonComponent buttontext="Register"/>
    </div>
    <div class="humberge">
      <div></div>
      <div></div>
    </div>
  </div>
</template>
<style scoped>
  .navbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5rem;

  }
  .logodiv{
    text-decoration: none;
    color: #fff;
    display: flex;
    gap: 5px;
    align-items: center;
  }
  .navbuttons, .links, .logotext{
    display: none;
  }
  .humberge div{
    width: 30px;
    height: 5px;
    margin-bottom: 5px;
    background-color: #fff;
  }
  @media (min-width: 769px) {
    .humberge{
    display: none;
  }
  .logotext{
    color: #FFF;
    text-align: center;
    font-family: 'Ubuntu';
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: 24px;
    display: block;
  }
   .navbuttons, .links{
    display: flex;
    gap: 10px;
    align-items: center;
  } 
  .link-item{
      color: #FFF;
      text-align: center;
      font-family: 'Ubuntu';
      font-size: 18px;
      font-style: normal;
      font-weight: 400;
      line-height: 18px;
      text-decoration: none;
  }    
  }
</style>