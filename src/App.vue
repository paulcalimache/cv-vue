<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <main>
    <div id="notch"></div>
    <a id="backHome" href="/" v-if="$route.name !== 'home'"><img src="https://www.svgrepo.com/show/77532/left-arrow-sketch.svg" width="40" height="40"></a>
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
  position:relative;
  overflow-x: hidden;
  overflow-y: scroll;
}
main::-webkit-scrollbar {
  display: none;
}

#notch {
  position: fixed;
  left:50%;
  transform: translateX(-50%);
  width:180px;
  height:20px;
  border-radius: 0 0 15px 15px;
  background-color: black;
  z-index: 1;
}
#backHome {
  position:fixed;
  left:inherit;
  margin-left:10px;
  margin-top:10px;
  z-index:2;
}
a {
  text-decoration: none;
}
a::after {
  text-decoration: none;
}
</style>
