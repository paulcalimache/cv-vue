<script>
  export default {
    props: ['title']
  }
</script>

<template>
  <div class="appIcon">
    <span class="appIcon-title">{{ title }}</span>
  </div>
</template>

<style scoped>
  .appIcon {
    width:90px;
    height:90px;
    border-radius: 25px;
    background:rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }
  .appIcon-title{
    color:white;
  }
</style>