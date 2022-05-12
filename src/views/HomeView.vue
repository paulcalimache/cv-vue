<script setup>
import appIcon from '@/components/appIcon.vue';
let aboutTitle = 'About'; let aboutIcon = '/Icons/paper.svg'; let aboutColor = 'rgb(38, 70, 83)';
let worksTitle = 'Works'; let worksIcon = '/Icons/works-box.svg'; let worksColor = 'rgb(247, 214, 224)'
let contactTitle = 'Contact'; let contactIcon = '/Icons/contact-mail-red.svg'; let contactColor = 'rgb(177, 221, 241)';
let linkedinTitle = 'Linkedin'; let linkedinIcon = '/Icons/LinkedIn.png'; let linkedinColor = 'rgb(0, 127, 188)';
let githubTitle = 'Github'; let githubIcon = '/Icons/github.png'; let githubColor = 'black';

</script>

<template>
  <div id="home">
    <a href="/about"><appIcon :title="aboutTitle" :icon="aboutIcon" :bgcolor="aboutColor"/></a>
    <a href="/works"><appIcon :title="worksTitle" :icon="worksIcon" :bgcolor="worksColor"/></a>
    <a href="/contact"><appIcon :title="contactTitle" :icon="contactIcon" :bgcolor="contactColor"/></a>
    <a href="https://github.com/paulcalimache" target="_blank"><appIcon :title="githubTitle" :icon="githubIcon" :bgcolor="githubColor"/></a>
    <a href="https://www.linkedin.com/in/paul-calimache/" target="_blank"><appIcon :title="linkedinTitle" :icon="linkedinIcon" :bgcolor="linkedinColor"/></a>
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
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows:min-content min-content;
    row-gap:40px;
  }
</style>