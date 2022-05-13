<template>
  <div id="about">
    <div class="about-image">
      <img src="/Icons/profile-illustration.png">
    </div>
    <div id="about-body">
      <div class="about-name">
        <span class="name">Paul</span>
        <span class="name">Calimache</span>
        <div class="about-actively">
          <span class="looking">Actively looking for internship</span>
          <img src="/Icons/eye.gif" width="100px" alt="This will display an animated GIF"/>
        </div>
      </div>
      <div class="about-profile">
        <div class="profile-cta">
          <div>
            <span class="discover">Discover my profile</span>
            <span class="discover-cats">Education | Job Experience | Skills</span>
          </div>
          <svg class="arrows">
            <path class="a1" d="M0 0 L15 16 L30 0"></path>
            <path class="a2" d="M0 10 L15 26 L30 10"></path>
            <path class="a3" d="M0 20 L15 36 L30 20"></path>
          </svg>
        </div>
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
    padding-top:20px;
  }
  .about-name {
    margin-left:20px;
  }
  .name {
    color:black;
    display:block;
    font-size:26px;
  }
  .about-actively {
    display:flex;
    align-items: center;
  }
  .looking {
    font-size:18px;
    color:rgb(81, 167, 251);
  }
  /* ################## */
  .about-profile {
    margin-top:10px;
    background-color:rgb(81, 167, 251);
    border-radius:20px 20px 0 0;
    padding-top:20px;
    height:100vh;
    padding-left:20px;
  }

  .profile-cta {
    display:flex;
    column-gap:40px;
    align-items: center;
  }
  .discover {
    display:block;
    font-size:18px;
    color:black;
  }
  .discover-cats {
    color:black;
    display:block;
  }
  .arrows {
	width: 30px;
	height: 36px;
}

.arrows path {
	stroke: rgba(0, 0, 0, 0.8);
	fill: transparent;
	stroke-width: 1px;	
	animation: arrow 3s infinite;
	-webkit-animation: arrow 3s infinite; 
}

@keyframes arrow
{
0% {opacity:0}
40% {opacity:1}
80% {opacity:0}
100% {opacity:0}
}

@-webkit-keyframes arrow /*Safari and Chrome*/
{
0% {opacity:0}
40% {opacity:1}
80% {opacity:0}
100% {opacity:0}
}

.arrows path.a1 {
	animation-delay:-1s;
	-webkit-animation-delay:-1s; /* Safari 和 Chrome */
}

.arrows path.a2 {
	animation-delay:-0.5s;
	-webkit-animation-delay:-0.5s; /* Safari 和 Chrome */
}

.arrows path.a3 {	
	animation-delay:0s;
	-webkit-animation-delay:0s; /* Safari 和 Chrome */
}
</style>
