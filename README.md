<svg viewBox="0 0 115 25" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">

<style>

svg text {
  transform-origin: 50% 50%;
  transform: translate(0%, -40%) rotate(180deg);
}

svg image {
  transform-origin: 50% 50%;
  transform: translate(0%, -40%) rotate(180deg);
}

svg {
  width:100vw;
  position:fixed;
  top:-5px;
  transform: rotate(180deg);
  overflow:visible;
}

rect.headerRect {
  fill: black;
  fill-opacity: 20%;
}
rect.headerRect:hover {
  fill: yellow;
  fill-opacity: 50%;
}

.wave {
  animation: wave 3s linear;
  animation-iteration-count:infinite;
  fill: #2620F6;  
}

.wave:hover {
  fill: #2620F6;
}

.drop:hover {
  fill: #C9FFE5;
}

.drop {
  fill: #231279;
  xfill: #1D1233;
  animation: drop 8.2s linear infinite normal;
  stroke: #231279;
  stroke-width: 0.5;
  transform: translateY(25px) ;
  transform-box: fill-box;
  transform-origin: 50% 100%;
}
.drop1 {
}

.drop2 {
  animation-delay: 3s;
  animation-duration:5s;
}
.drop3 {
  animation-delay: -2s;
  animation-duration:5.4s;
}
.drop4 {
  animation-delay: 1.7s;
  animation-duration:2.4s;
}
.drop5 {
  animation-delay: 2.7s;
  animation-duration:5.1s;
}
.drop6 {
  animation-delay: -2.1s;
  animation-duration:5.2s;
}
.gooeff {
  	filter: url(#goo);
}
#wave2 {
  animation-duration:5s;
  animation-direction: reverse;
  opacity: .6
}
#wave3 {
  animation-duration: 7s;
  opacity:.3;
}
@keyframes drop {
  0% {
    transform: translateY(25px); 
  }
  30% {
    transform: translateY(-10px) scale(.1);
  }
  30.001% {
    transform: translateY(25px) scale(1); 
  }
  70% {
    transform: translateY(25px); 
  }
  100% { 
    transform: translateY(-15px) scale(.1);  
  }
}
@keyframes wave {
  to {transform: translateX(-100%);}
}
@keyframes blink {
  0% {
    fill: #FFFFFF;
  }
  100% {
    fill: none;
  }
}
@keyframes underline_move {
  to {
    transform: translateX(-39px);
  }}

g.typingUnderline rect {
   animation: 
    blink 0.5s infinite, 
    underline_move 4s steps(24, end) forwards;
}
</style>
 <defs> 
    <filter id="goo">
      <feGaussianBlur in="SourceGraphic" stdDeviation="1" result="blur" />
      <feColorMatrix in="blur" mode="matrix" values="
           1 0 0 0 0  
           0 1 0 0 0  
           0 0 1 0 0  
           0 0 0 13 -9" result="goo" />
      <xfeBlend in="SourceGraphic" in2="goo" />
  	</filter>
   
    <path id="wave" d="M 0,10 C 30,10 30,15 60,15 90,15 90,10 120,10 150,10 150,15 180,15 210,15 210,10 240,10 v 28 h -240 z" />
  </defs> 

  <rect fill="#AAA" fill-opacity="50%" x="0" y="1" width="100%" height="0.4" ></rect>
 
  <use id="wave3" class="wave" xlink:href="#wave" x="0" y="-2" ></use> 
  <use id="wave2" class="wave" xlink:href="#wave" x="0" y="0" ></use>
 
  <g class="gooeff" filter="url(#goo)">
    <circle class="drop drop1" cx="95" cy="2" r="8.8"  />
    <circle class="drop drop2" cx="35" cy="2.5" r="7.5"  />
    <circle class="drop drop3" cx="26" cy="2.8" r="9.2"  />
    <circle class="drop drop4" cx="14" cy="2" r="8.8"  />
    <circle class="drop drop5" cx="22" cy="2.5" r="7.5"  />
    <circle class="drop drop6" cx="6" cy="2.8" r="9.2"  />
      
    <circle class="drop drop1" cx="45" cy="4.4" r="8.8"  />
    <circle class="drop drop2" cx="99" cy="4.1" r="7.5"  />
    <circle class="drop drop3" cx="8" cy="3.8" r="9.2"  />
    <circle class="drop drop4" cx="3" cy="4.4" r="8.8"  />
    <circle class="drop drop5" cx="7" cy="4.1" r="7.5"  />
    <circle class="drop drop6" cx="10" cy="4.3" r="9.2"  />
    
    <circle class="drop drop1" cx="32" cy="5.4" r="8.8"  />
    <circle class="drop drop2" cx="5.2" cy="5.1" r="7.5"  />
    <circle class="drop drop3" cx="0.2" cy="5.3" r="9.2"  />
    <circle class="drop drop4" cx="3.2" cy="5.4" r="8.8"  />
    <circle class="drop drop5" cx="14.2" cy="5.1" r="7.5"  />
    <circle class="drop drop6" cx="17.2" cy="4.8" r="9.2"  />
      
    <use id="wave1" class="wave" xlink:href="#wave" x="0" y="1" />
  </g>  

<rect class="headerRect" width="70" height="7.3" rx="1" x="20" y="16.8"/>

<path id="nameTyping">
  <animate attributeName="d" from="m38,-5 h0" to="m38,-5 h100" dur="9.4s" begin="0s" fill="freeze"/>
</path>

<text font-family="Courier New" font-size=".22em" fill="white"
      font-weight="bold" letter-spacing="0.5">
  <textPath xlink:href="#nameTyping" >
      Hi, I am Vanessa!
  </textPath>
</text>

<g class="typingUnderline">
  <rect fill="#FFFFFF" x="70" y="20.5" width="2.5" height="0.4" xlink:href="#underlineTyping">
      <animate attributeName="visible" from="hidden" to="visible" dur="1s" fill="freeze"/>
  </rect>
</g>

<path id="descriptionTyping">
  <animate attributeName="d" from="m30,-3 h0" to="m30,-3 h100" 
           dur="5.8s" begin="0s" fill="freeze"/>
</path>
</svg>

- Atualmente trabalhando no back-end Node Js., Typescript e Prisma ORM
- Estudando React Native

<div align="center">
  <a href="https://github.com/luis-procopio">
    <img height="150em" width="40%" src="https://github-readme-stats.vercel.app/api?username=luis-procopio&count_private=true&include_all_commits=true&show_icons=true&theme=dracula&hide_border=false&show_owner=true"/>
    <img height="150em" width="40%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=luis-procopio&theme=dracula&hide_border=false&&layout=compact"/>
  </a>
</div>
 
 <div align="center" valign="top"><br>
  <img align="center" alt="Luis-Ts" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" />
  <img align="center" alt="Luis-Node" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" />
  <img align="center" alt="Luis-Prisma" height="30" width="35" src="https://user-images.githubusercontent.com/108732662/220519454-a2a0001b-b173-427f-83da-1506b0eabbe2.png" />
  <img align="center" alt="Luis-React" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" />
 </div>
 
 
