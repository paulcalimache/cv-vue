<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <main>
    <div id="notch"></div>
    <RouterView />
  </main>
</template>

<style>
@import '@/assets/base.css';

#app {
  height:100vh;
  widows: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(217, 201, 191);
}

main {
  width:400px;
  height: 650px;
  border:5px black solid;
  border-radius: 30px;
  overflow: hidden;
  position:relative;
}

#notch {
  position: absolute;
  left:50%;
  transform: translateX(-50%);
  width:180px;
  height:20px;
  border-radius: 0 0 15px 15px;
  background-color: black;
  z-index: 1;
}

</style>
