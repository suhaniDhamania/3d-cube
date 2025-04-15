# 3d-cube

*key point
.cube{
    width: 100%;
  height: 100%;
    transform-style: preserve-3d;
    position:relative;
    animation: rotate 5s infinite linear;
}
.front  { transform: translateZ(50px); }
.back   { transform: rotateY(180deg) translateZ(50px); }
.right  { transform: rotateY(90deg) translateZ(50px); }
.left   { transform: rotateY(-90deg) translateZ(50px); }
.top    { transform: rotateX(90deg) translateZ(50px);}
.bottom { transform: rotateX(-90deg) translateZ(50px); }

.cube:hover {
    animation-play-state: paused;
  }
  
@keyframes rotate {
    0% {
      transform: rotateX(0) rotateY(0);
    }
    100% {
      transform: rotateX(360deg) rotateY(360deg);
    }
  }
  
