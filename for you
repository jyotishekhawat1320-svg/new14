<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Ronak 💗</title>
<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Nunito:wght@400;600&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;}
body{
  height:100vh;
  background:radial-gradient(circle at top,#2b0015,#12000a);
  font-family:'Nunito',sans-serif;
  overflow:hidden;
  color:#ffd6e8;
}
/* floating hearts */
.heart{
  position:absolute;
  font-size:18px;
  opacity:0.6;
  animation: float 6s linear infinite;
  pointer-events:none;
}
@keyframes float{
  from{transform:translateY(110vh);}
  to{transform:translateY(-10vh);}
}
/* pages */
.page{
  display:none;
  height:100vh;
  width:100%;
  align-items:center;
  justify-content:center;
  text-align:center;
}
.page.active{display:flex;}
.box{
  background:linear-gradient(145deg,#3a001e,#1a000d);
  padding:38px;
  border-radius:26px;
  max-width:700px;
  box-shadow:0 30px 80px rgba(255,20,120,0.45);
  animation: open 0.9s ease;
}
@keyframes open{
  from{transform:scale(0.8);opacity:0;}
  to{transform:scale(1);opacity:1;}
}
h1{
  font-family:'Great Vibes',cursive;
  font-size:3.4rem;
  color:#ff77aa;
}
p{
  font-size:1.25rem;
  line-height:1.8;
  margin-top:18px;
}
button{
  margin-top:26px;
  padding:13px 34px;
  border:none;
  border-radius:40px;
  background:#ff4f9a;
  color:white;
  font-size:1.1rem;
  cursor:pointer;
  transition:0.3s;
}
button:hover{transform:scale(1.12);}
#no{position:absolute;}
/* envelope */
.envelope{
  width:350px;
  height:240px;
  background:#ff4f9a;
  border-radius:14px;
  position:relative;
  cursor:pointer;
  box-shadow:0 30px 80px rgba(255,0,120,0.6);
}
.flap{
  position:absolute;
  width:100%;
  height:50%;
  background:#ff2f7f;
  clip-path:polygon(0 0,100% 0,50% 100%);
  transform-origin:top;
  transition:0.8s;
}
.envelope:hover .flap{transform:rotateX(180deg);}
.env-text{
  position:absolute;
  bottom:30px;
  width:100%;
  color:white;
  font-family:'Great Vibes',cursive;
  font-size:2.4rem;
}
/* ring */
.ring{
  font-size:70px;
  animation: ringPop 1.2s ease infinite alternate;
}
@keyframes ringPop{
  from{transform:scale(1);}
  to{transform:scale(1.2);}
}
/* poppers */
.popper{
  position:absolute;
  font-size:26px;
  animation: pop 4s linear forwards;
}
@keyframes pop{
  to{transform:translateY(110vh);opacity:0;}
}
</style>
</head>
<body>
<!-- MUSIC -->
<audio id="music" loop>
  <source src="https://cdn.pixabay.com/download/audio/2023/03/20/audio_f3c3a0a4c0.mp3" type="audio/mpeg">
</audio>
<script>
for(let i=0;i<30;i++){
  let h=document.createElement("div");
  h.className="heart";
  h.innerHTML="💗";
  h.style.left=Math.random()*100+"%";
  h.style.animationDuration=4+Math.random()*5+"s";
  document.body.appendChild(h);
}
</script>

<!-- PAGE 1: Envelope -->
<div class="page active">
  <div class="envelope" onclick="start()">
    <div class="flap"></div>
    <div class="env-text">For You Ronak 💌</div>
  </div>
</div>

<!-- DAYS -->
<div class="page"><div class="box"><h1>Pre-Pre-Valentine Wish 💕</h1><p>FOR MY BOYFRIEND 💕</p><button onclick="next()">Next 💞</button></div></div>

<div class="page"><div class="box"><h1>🌹 Rose Day</h1><p>No rose is more pretty and precious than my FOOL😭 🌸</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>💍 Propose Day</h1><p>Would you like to stay with me little longer my love?🥰</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>🍫 Chocolate Day</h1><p>chocolate se bhi zyada sweet hai tu 😚</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>🧸 Teddy Day</h1><p>My baby is much more cutie than teddy so no need of teddy 😉😽</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>🤞 Promise Day</h1><p>I promise I am always with you baby jii🤗</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>🤗 Hug Day</h1><p>ab Can't wait to hug you by myself😭🥺🫂</p><button onclick="next()">Next</button></div></div>

<div class="page"><div class="box"><h1>💋 Kiss Day</h1><p>muuuaaaawwwwhhh💕baaki milkar 😺💋</p><button onclick="next()">Next</button></div></div>

<!-- QUESTION -->
<div class="page">
  <div class="box">
    <h1> 💘Valentine Day</h1>
    <p> So asking you offically<br> Will you be my Valentine?🥺 </p>
    <button onclick="yes()">YES 💖</button>
    <button id="no">NO 🙃</button>
  </div>
</div>

<!-- FINAL -->
<div class="page">
  <div class="box">
    <div class="ring">💍</div>
    <p id="type"></p>
  </div>
</div>

<script>
const pages=document.querySelectorAll('.page');
let i=0;
function start(){ 
  document.getElementById("music").play(); 
  next(); 
}
function next(){ 
  pages[i].classList.remove('active'); 
  i++; 
  pages[i].classList.add('active'); 
}
document.getElementById("no").onmouseover=()=>{
  const b=document.getElementById("no");
  b.innerText=["Wrong 😏","Try again 😤","Only YES 😌","Nice try 😎"][Math.floor(Math.random()*4)];
  b.style.left=Math.random()*80+"%";
  b.style.top=Math.random()*70+"%";
};
function yes(){
  alert("ab toh aap officially booked ho baby jii 💍😌");
  next();
  typing();
  for(let i=0;i<60;i++){
    let p=document.createElement("div");
    p.className="popper";
    p.innerHTML=["🎉","💖","✨","🥰"][Math.floor(Math.random()*4)];
    p.style.left=Math.random()*100+"%";
    p.style.top="-20px";
    document.body.appendChild(p);
    setTimeout(()=>p.remove(),4000);
  }
}

/* typing letter */
const text="Happy Valentine’s Day my baby 💖 I just want to say I am super happy to have you in my life🫶 I love you today tommorrow and always❤️... And also super proud of you 🤗 my boy I know you are going to achieve lot of things... and me also🌟 A REMINDER MY LOVE 🌸🌷 Main hmesha Tera wait karti rahungi ⏳ Tujhe pyaar krti rahungi 💖 And obvious😙 hamesha tere saath hi rahungiii 💕 Tu bestest friend hai mera, My home,happy place,peace OR mera future bhi Basically my everthing 🥺🌍✨";
let idx=0;
function typing(){
  const t=document.getElementById("type");
  if(idx<text.length){
    t.innerHTML+=text.charAt(idx);
    idx++;
    setTimeout(typing,38);
  }
}
</script>
</body>
</html>
