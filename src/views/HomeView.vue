<script setup>
import appIcon from '@/components/appIcon.vue';
let contactTitle = 'Contact';
let worksTitle = 'Works';
</script>

<template>
  <div id="home">
    <appIcon :title="contactTitle"/>
    <appIcon :title="worksTitle"/>
    <appIcon :title="contactTitle"/>
  </div>
</template>

<style scoped>
  #home {
    width:100%;
    height: 100%;
    background-image: url(../assets/wallpaper/POOL_DAY_QUEER_BEAR.jpg);
    background-position: center;
    background-size: cover;
    padding-top:40px;
    display: flex;
    justify-content: space-evenly;
  }
</style>