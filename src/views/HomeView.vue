<script setup>
import appIcon from '@/components/appIcon.vue';
let aboutTitle = 'About'; let aboutIcon = 'src/assets/Icons/paper.svg'; let aboutColor = 'rgb(38, 70, 83)';
let worksTitle = 'Works'; let worksIcon = 'src/assets/Icons/works-box.svg'; let worksColor = 'rgb(247, 214, 224)'
let contactTitle = 'Contact'; let contactIcon = 'src/assets/Icons/contact-mail-red.svg'; let contactColor = 'rgb(177, 221, 241)';
let linkedinTitle = 'Linkedin';
let githubTitle = 'Github';

</script>

<template>
  <div id="home">
    <a href="/about"><appIcon :title="aboutTitle" :icon="aboutIcon" :bgcolor="aboutColor"/></a>
    <a href="/works"><appIcon :title="worksTitle" :icon="worksIcon" :bgcolor="worksColor"/></a>
    <a href="/contact"><appIcon :title="contactTitle" :icon="contactIcon" :bgcolor="contactColor"/></a>
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
    align-items:flex-start;
  }

  a {
    text-decoration: none;
  }
  a::after {
    text-decoration: none;
  }
</style>