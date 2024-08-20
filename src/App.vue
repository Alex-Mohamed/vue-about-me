<script setup>
  import WebHeader from './components/WebHeader.vue'
  import AboutMe from './components/AboutMe.vue';
</script>

<template>
  <header>
    <img id="pic" alt="Alex Mohamed" height="500" class="logo" src="./assets/about_me.jpeg"/>
  </header>
 
 
  <div class="wrapper">
    <WebHeader msg="About Me: Alex Mohamed" />
    <p>&emsp;</p>
    <AboutMe/>
  </div>
</template>
 
 
 <style scoped>
  .logo {
    display: block;
    margin: 0 auto 2rem;
    position: relative;
  }
 
 
  @media (min-width: 1024px) {
    header {
      line-height: 1.5;
      display: flex;
      justify-content:center;
      padding-right: calc(var(--section-gap) / 2);
    }
 
 
    .logo {
      display: block;
      margin: 0 auto 2rem;
      position: relative;
    }
  }
 </style>
 