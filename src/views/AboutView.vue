<script setup>
  import profile from '@/components/profile.vue';
</script>

<template>
  <div id="about">
    <div class="about-image">
      <img src="/Icons/profile-illustration.png">
    </div>
    <div id="about-body">
      <div class="about-name">
        <span class="name">Paul Calimache</span>
        <span class="situation">French IT student.</span>
        <div class="about-actively">
          <span class="looking">Actively looking for internship</span>
          <img src="/Icons/eye.gif" width="100px" alt="This will display an animated GIF"/>
        </div>
      </div>
      <div class="about-profile">
        <profile />
      </div>
    </div>
  </div>
</template>

<style scoped>
  #about {
    background:white;
  }
  .about-image {
    position:sticky;
    top:0;
    width:100%;
    padding-top:20px;
  }
  #about-body {
    background:white;
    border-radius:20px 20px 0 0;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.8);
    width:100%;
    padding-top:10px;
  }
  .about-name {
    margin-left:20px;
  }
  .name {
    color:black;
    display:block;
    font-size:26px;
    font-weight:bold;
  }
  .situation {
    display:block;
    font-size:26px;
    font-weight:lighter;
  }
  .about-actively {
    display:flex;
    align-items: center;
  }
  .looking {
    font-size:18px;
    font-weight:bold;
    color:rgb(81, 167, 251);
  }
  .about-profile {
    margin-top:10px;
    background-color:rgb(81, 167, 251);
    border-radius:20px 20px 0 0;
    padding-top:20px;
    height:100vh;
    padding-left:20px;
    padding-right: 20px;
  }
</style>
