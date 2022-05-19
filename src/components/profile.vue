<template>
    <div class="profile-cta">
        <div>
            <span class="discover">Discover my profile</span>
            <span class="discover-cats">Profile | Education & Experience | Skills</span>
        </div>
        <svg class="arrows">
            <path class="a1" d="M0 0 L15 16 L30 0"></path>
            <path class="a2" d="M0 10 L15 26 L30 10"></path>
            <path class="a3" d="M0 20 L15 36 L30 20"></path>
        </svg>
    </div>
    <div class="profile-intro">
        <div class="intro-text">
            <h2>Hello !</h2>
            <span>I’m Paul Calimache,</span> 
            <span>
                A 21 years old french student living in Toulouse.
                Actually I'm studying IT in an engineer school named CESI and also I'm working in apprenticeship as software engineer at Thales Alenia Space a space company.
            </span>
            <h2 class="lookingfor">Looking for ...</h2>
            <span>To validate my degree I have to do an internship in another country.</span>
            <span>
                If your company is in IT world and looking for an intership you can contact me through the <a href="/contact">contact page</a>.
            </span>
        </div>
        <div class="WhatIdo">
            What I do :
        </div>
    </div>
</template>

<style scoped>
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
/* ------------------------------------------------------------------------ */
.profile-intro {
    margin-top:40px;
}
.intro-text {
    color:black;
    font-weight:lighter;
    text-align: justify;
    display:flex;
    flex-direction:column;
}
.lookingfor{
    margin-top:40px;
}

</style>