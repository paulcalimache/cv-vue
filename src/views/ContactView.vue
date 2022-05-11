<script setup>
</script>

<template>
  <div id="contact">
    <div class="contact-header">
      <lottie-player src="https://assets2.lottiefiles.com/packages/lf20_in4cufsz.json"  background="transparent"  speed="1"  style="width: 250px; height: 200px;"  loop autoplay></lottie-player>
    </div>
    <div class="contact-body">
      <div class="contact-row"><span class="label">TO:</span></div>
      <div class="contact-row"><label for="email">FROM:</label><input type="email" id="email" name="email"></div>
      <div class="contact-row"><label for="subject">SUBJECT:</label><input type="text" id="subject" name="subject"></div>
      <div class="contact-row"><label for="subject">MESSAGE:</label></div>
      <textarea type="email" id="email" name="email"></textarea>
    </div>
  </div>
</template>

<style>
#contact {
    width:100%;
    height:100%;
    background:rgb(255, 255, 255);
}
.contact-header {
  display:flex;
    justify-content: center;
    position:relative;
    background:green;
}
.contact-body {
  width:100%;
  height:100%;
}
.contact-row {
  width:100%;
  border-top:5px black solid;
  padding:5px;
  display:flex;
  justify-content: space-between;
  column-gap:5px;
  align-items: center;
}
label, .label {
  color:green;
  font-weight: bold;
}
input, textarea {
  flex-grow: 1;
  border:0;
  outline:none;
}
textarea {
  width:100%;
  height:300px;
  overflow-y:hidden;
  resize: none;
}
</style>