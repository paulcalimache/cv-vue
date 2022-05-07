<script>
  export default {
    props: ['title','icon','bgcolor'],
  };

</script>

<template>
  <div class="appIcon">
    <div class="appIcon-item" :style="{'background': bgcolor}">
      <img :src="icon"/>
    </div>
    <span class="appIcon-title">{{ title }}</span>
  </div>
</template>

<style scoped>
.appIcon {
  display: flex;
  flex-direction: column;
  align-items:center;
}
.appIcon:hover {
  cursor:pointer;
  transform:scale(1.1);
}

.appIcon-item {
  width:90px;
  height:90px;
  border-radius: 25px;
  display:flex;
  justify-content:center;
  align-items:center;
}
img {
  width:80px;
  height:80px;
}
.appIcon-title{
  color:white;
  font-weight: bold;
}
</style>