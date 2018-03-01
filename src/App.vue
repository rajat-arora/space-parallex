<template>
  <div id="app">
    <div id="scene" class="scene unselectable" data-friction-x="0.1"
			data-friction-y="0.1"
			data-scalar-x="25"
			data-scalar-y="15">
      <li class="layer" data-depth="0.00"></li>
			<li class="layer" data-depth="0.10"><div class="background"></div></li>

       	<li class="layer" data-depth="0.15">
          <div class="star0 star-move1"> <img src="./assets/images/stars.png" alt="Rope"></div>

           <div class="star1 star-move"> <img src="./assets/images/stars.png" alt="Rope"></div>
          <div class="star2 star-move1"> <img src="./assets/images/stars.png" alt="Rope"></div>
          <div class="star3 star-move"> <img src="./assets/images/stars.png" alt="Rope"></div>
          <div class="star4 star-move"> <img src="./assets/images/stars.png" alt="Rope"></div>
          <div class="star5 star-move1"> <img src="./assets/images/stars.png" alt="Rope"></div>
          <div class="star6 star-move"> <img src="./assets/images/stars.png" alt="Rope"></div>

			</li>
            

 	<li class="layer" data-depth="0.20">
				<ul class="rope depth-10">
					<li><img src="./assets/images/rope.png" alt="Rope"></li>
					<li class="hanger position-2">
						<div class="board cloud-2 swing-1"></div>
					</li>
					<li class="hanger position-4">
						<div class="board cloud-1 swing-3"></div>
					</li>
					<li class="hanger position-8">
						<div class="board birds swing-5"></div>
					</li>
				</ul>
			</li>

      <li class="layer" data-depth="0.60">
				<ul class="rope depth-60">
					<li><img src="./assets/images/rope.png" alt="Rope"></li>
					<li class="hanger position-3">
						<div class="board birds swing-5"></div>
					</li>
					<li class="hanger position-6">
						<div class="board cloud-2 swing-2"></div>
					</li>
					<li class="hanger position-8">
						<div class="board cloud-3 swing-4"></div>
					</li>
				</ul>
			</li>

      <li class="layer" data-depth="0.70">
          <div class="ship"> <img src="./assets/images/space-ship.png" alt="Rope"></div>
			</li>
          <li class="layer" data-depth="0.80">
          <div class="footer">Made with 🚀 by Rajat</div>
			</li>
</div>
  </div>
</template>

<script>
import Parallax from 'parallax-js'
export default {
  name: 'app',
  data () {
    return {
    }
  },
  mounted(){
    var scene = document.getElementById('scene');
var parallaxInstance = new Parallax(scene);
  }
}
</script>

<style>

@-webkit-keyframes phase {
  0% {
    opacity: 1; }
  25% {
    opacity: 0.4; }
  50% {
    opacity: 0.8; }
  75% {
    opacity: 0.4; }
  100% {
    opacity: 1; } }
@-moz-keyframes phase {
  0% {
    opacity: 1; }
  25% {
    opacity: 0.4; }
  50% {
    opacity: 0.8; }
  75% {
    opacity: 0.4; }
  100% {
    opacity: 1; } }
@-ms-keyframes phase {
  0% {
    opacity: 1; }
  25% {
    opacity: 0.4; }
  50% {
    opacity: 0.8; }
  75% {
    opacity: 0.4; }
  100% {
    opacity: 1; } }
@keyframes phase {
  0% {
    opacity: 1; }
  25% {
    opacity: 0.4; }
  50% {
    opacity: 0.8; }
  75% {
    opacity: 0.4; }
  100% {
    opacity: 1; } }
@-webkit-keyframes tilt {
  0% {
    -webkit-transform: rotateX(-30deg);
    -moz-transform: rotateX(-30deg);
    transform: rotateX(-30deg); }
  25% {
    -webkit-transform: rotateX( 30deg);
    -moz-transform: rotateX( 30deg);
    transform: rotateX( 30deg); }
  50% {
    -webkit-transform: rotateY(-30deg);
    -moz-transform: rotateY(-30deg);
    transform: rotateY(-30deg); }
  75% {
    -webkit-transform: rotateY( 30deg);
    -moz-transform: rotateY( 30deg);
    transform: rotateY( 30deg); }
  100% {
    -webkit-transform: rotateZ( 20deg);
    -moz-transform: rotateZ( 20deg);
    transform: rotateZ( 20deg); } }
@-moz-keyframes tilt {
  0% {
    -webkit-transform: rotateX(-30deg);
    -moz-transform: rotateX(-30deg);
    transform: rotateX(-30deg); }
  25% {
    -webkit-transform: rotateX( 30deg);
    -moz-transform: rotateX( 30deg);
    transform: rotateX( 30deg); }
  50% {
    -webkit-transform: rotateY(-30deg);
    -moz-transform: rotateY(-30deg);
    transform: rotateY(-30deg); }
  75% {
    -webkit-transform: rotateY( 30deg);
    -moz-transform: rotateY( 30deg);
    transform: rotateY( 30deg); }
  100% {
    -webkit-transform: rotateZ( 20deg);
    -moz-transform: rotateZ( 20deg);
    transform: rotateZ( 20deg); } }
@-ms-keyframes tilt {
  0% {
    -webkit-transform: rotateX(-30deg);
    -moz-transform: rotateX(-30deg);
    transform: rotateX(-30deg); }
  25% {
    -webkit-transform: rotateX( 30deg);
    -moz-transform: rotateX( 30deg);
    transform: rotateX( 30deg); }
  50% {
    -webkit-transform: rotateY(-30deg);
    -moz-transform: rotateY(-30deg);
    transform: rotateY(-30deg); }
  75% {
    -webkit-transform: rotateY( 30deg);
    -moz-transform: rotateY( 30deg);
    transform: rotateY( 30deg); }
  100% {
    -webkit-transform: rotateZ( 20deg);
    -moz-transform: rotateZ( 20deg);
    transform: rotateZ( 20deg); } }
@keyframes tilt {
  0% {
    -webkit-transform: rotateX(-30deg);
    -moz-transform: rotateX(-30deg);
    transform: rotateX(-30deg); }
  25% {
    -webkit-transform: rotateX( 30deg);
    -moz-transform: rotateX( 30deg);
    transform: rotateX( 30deg); }
  50% {
    -webkit-transform: rotateY(-30deg);
    -moz-transform: rotateY(-30deg);
    transform: rotateY(-30deg); }
  75% {
    -webkit-transform: rotateY( 30deg);
    -moz-transform: rotateY( 30deg);
    transform: rotateY( 30deg); }
  100% {
    -webkit-transform: rotateZ( 20deg);
    -moz-transform: rotateZ( 20deg);
    transform: rotateZ( 20deg); } }
    @-webkit-keyframes swing {
  0% {
    -webkit-transform: rotateZ(10deg);
    -moz-transform: rotateZ(10deg);
    transform: rotateZ(10deg); }
  100% {
    -webkit-transform: rotateZ(-10deg);
    -moz-transform: rotateZ(-10deg);
    transform: rotateZ(-10deg); } }
@-moz-keyframes swing {
  0% {
    -webkit-transform: rotateZ(10deg);
    -moz-transform: rotateZ(10deg);
    transform: rotateZ(10deg); }
  100% {
    -webkit-transform: rotateZ(-10deg);
    -moz-transform: rotateZ(-10deg);
    transform: rotateZ(-10deg); } }
@-ms-keyframes swing {
  0% {
    -webkit-transform: rotateZ(10deg);
    -moz-transform: rotateZ(10deg);
    transform: rotateZ(10deg); }
  100% {
    -webkit-transform: rotateZ(-10deg);
    -moz-transform: rotateZ(-10deg);
    transform: rotateZ(-10deg); } }
@keyframes swing {
  0% {
    -webkit-transform: rotateZ(10deg);
    -moz-transform: rotateZ(10deg);
    transform: rotateZ(10deg); }
  100% {
    -webkit-transform: rotateZ(-10deg);
    -moz-transform: rotateZ(-10deg);
    transform: rotateZ(-10deg); } }
html.mouse a:hover, html.mouse button:hover {
  -webkit-transition: color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), background-color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), opacity 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
  -moz-transition: color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), background-color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), opacity 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
  transition: color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), background-color 0.2s cubic-bezier(0.165, 0.84, 0.44, 1), opacity 0.2s cubic-bezier(0.165, 0.84, 0.44, 1); }
html.mouse a:hover {
  color: #ff755a; }
html.mouse button:hover {
  background-color: #D92400;
  color: #FFFFFF; }
html.mouse .toggle:hover .x, html.mouse .toggle:hover .y {
  background-color: #FFFFFF; }
html.mouse .links a:hover {
  background-color: #D92400;
  color: #FFFFFF; }

.scene,
.layer {
  display: block;
  height: 100vh;
  width: 100vw;
  padding: 0;
  margin: 0 ; }

.scene {
  min-height: 460px;
  position: relative;
  overflow: hidden; }

  .layer {
  position: absolute; }
  .layer div {
    -webkit-transform: translate3d(0,0,0);
    -moz-transform: translate3d(0,0,0);
    transform: translate3d(0,0,0);
    -webkit-transform-style: preserve-3d;
    -moz-transform-style: preserve-3d;
    transform-style: preserve-3d;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden; }
body{
  overflow: hidden !important;
}
    
.background {
  background: url(./assets/images/background.jpg) no-repeat 110% 100%;
  background-size: cover;
  position: absolute;
bottom: 96px;
  background-size: cover;
  position: absolute;
  width: 110%;
  height: 110%;

  left: -5%;
  top: -5%;
   }
    .star0{
  position: relative;
  left: 55%;
    top: 10%;

  }

  .star0 img {
  width: 5%;

  }

  .star1{
  position: relative;
  left: 15%;
    top: 10%;

  }

  .star1 img {
  width: 5%;

  }

  .star2{
  position: relative;
  left: 45%;
    top: 18%;

  }

  .star2 img {
  width: 5%;

  }


  .star3{
  position: relative;
  left: 85%;
    top: 50%;

  }

  .star3 img {
  width: 5%;

  }


  .star4{
  position: relative;
  left: 42%;
    top: 50%;

  }

  .star4 img {
  width: 5%;

  }


  .star5{
  position: relative;
  left: 15%;
    top: 20%;

  }

  .star5 img {
  width: 5%;

  }
  
    .star6{
  position: relative;
  left: 60%;
    top: -5%;

  }

  .star6 img {
  width: 5%;

  }

.rope {
  width: 115%;
  position: relative;
  left: -15%;
  position: relative; } 


.rope img {
  width: 120%;
   } 

.hanger {
  -webkit-transform-origin: 0% 0%;
  -moz-transform-origin: 0% 0%;
  transform-origin: 0% 0%;
  position: absolute; }
  .hanger.position-1 {
    top: 28%; }
  .hanger.position-2 {
    top: 40%; }
  .hanger.position-3 {
    top: 53%; }
  .hanger.position-4 {
    top: 61.5%;
     right: 50% !important; }
  .hanger.position-5 {
    top: 69.5%; }
  .hanger.position-6 {
    top: 68.5%; }
  .hanger.position-7 {
    top: 59%; }
  .hanger.position-8 {
    top: 61.5%; }
  .hanger.position-9 {
    top: 28%; }
  .hanger.position-1 {
    left: 10%; }
  .hanger.position-2 {
    left: 20%; }
  .hanger.position-3 {
    left: 30%; }
  .hanger.position-4 {
    left: 40%; }
  .hanger.position-5 {
    left: 50%; }
  .hanger.position-6 {
    left: 60%; }
  .hanger.position-7 {
    left: 70%; }
  .hanger.position-8 {
    left: 80%; }
  .hanger.position-9 {
    left: 90%; }
.board {
  -webkit-transform-origin: 50% 0%;
  -moz-transform-origin: 50% 0%;
  transform-origin: 50% 0%;
  margin: 0px -140px;
  background-size: 280px 280px;
  height: 280px;
  width: 280px;
  background-repeat: no-repeat;
  position: absolute;
  top: -4px;
  left: 0; }
  
  .board.birds {
    background-image: url(./assets/images/board-birds.png); }
  .board.cloud-1 {
    background-image: url(./assets/images/board-cloud-1.png); }
  .board.cloud-2 {
    background-image: url(./assets/images/board-cloud-2.png); }
  .board.cloud-3 {
    background-image: url(./assets/images/board-cloud-3.png); }
  .board.cloud-4 {
    background-image: url(./assets/images/board-cloud-4.png); }

  .swing-1 {
  -webkit-animation: swing 4s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  -moz-animation: swing 4s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  animation: swing 4s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important; }

.swing-2 {
  -webkit-animation: swing 3.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  -moz-animation: swing 3.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  animation: swing 3.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important; }

.swing-3 {
  -webkit-animation: swing 3s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important ;
  -moz-animation: swing 3s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  animation: swing 3s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955 ) !important; }

.swing-4 {
  -webkit-animation: swing 2.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  -moz-animation: swing 2.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  animation: swing 2.5s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important; }

.swing-5 {
  -webkit-animation: swing 2s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  -moz-animation: swing 2s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important;
  animation: swing 2s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955) !important; }

  .rope.depth-10 {
  -webkit-transform: scale(1);
  -moz-transform: scale(1);
  transform: scale(1);
  top: 20%; }
  .rope.depth-10 .hanger {
    -webkit-transform: scale(0.75);
    -moz-transform: scale(0.75);
    transform: scale(0.75); }

    rope.depth-60 {
  -webkit-transform: scale(1.13889);
  -moz-transform: scale(1.13889);
  transform: scale(1.13889);
  top: 3.33333%; }
  .rope.depth-60 .hanger {
    -webkit-transform: scale(0.85);
    -moz-transform: scale(0.85);
    transform: scale(0.85); }

    
dl,
menu,
ol,
ul {
  margin: 1em 0; }
  ul {
  list-style: none;
  display: block;
  padding: 0;
  margin: 0; }

.star-move {
    -webkit-animation: mover 1s infinite  alternate;
    animation: mover 1s infinite  alternate;
}
@-webkit-keyframes mover {
    0% { transform: translateY(0); }
    100% { transform: translateY(-20px); }
}
@keyframes mover {
    0% { transform: translateY(0); }
    100% { transform: translateY(-20px); }
}



.star-move1 {
    -webkit-animation: mover1 1s infinite  alternate;
    animation: mover1 1s infinite  alternate;
}
@-webkit-keyframes mover1 {
    0% { transform: translateY(-20); }
    100% { transform: translateY(0px); }
}
@keyframes mover1 {
    0% { transform: translateY(-20px); }
    100% { transform: translateY(0px); }
}

.ship{
  position: relative;
  left:60%;
    top: 65%;
    
}
.ship img{
  width: 10%;
}


.ship {
    -webkit-animation: ships 2s infinite  alternate;
    animation: ships 2s infinite  alternate;
}
@-webkit-keyframes ships {
    0% { transform: translateY(0); }

    100% { transform: translateY(-30px) translateX(50px); }
}
@keyframes ships {
    0% { transform: translateY(0); }
    100% { transform: translateY(-30px) translateX(50px); }
}

.footer{
    position: relative;
    color: white;
    font-size: 1.5em;
  left: 45%;
    top: 89%;
}

</style>
