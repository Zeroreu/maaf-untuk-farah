<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Untuk Farah 💖</title>
<style>
body{
  margin:0;
  font-family:'Poppins', sans-serif;
  background: linear-gradient(135deg,#ff9a9e,#fad0c4);
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
  overflow:hidden;
  text-align:center;
  color:white;
}
.gift-box{
  font-size:80px;
  cursor:pointer;
  transition:0.3s;
}
.gift-box:hover{
  transform:scale(1.1);
}
#letter{
  display:none;
  max-width:90%;
  animation:fadeIn 2s ease forwards;
}
button{
  padding:12px 25px;
  border:none;
  border-radius:25px;
  background:white;
  color:#ff6f91;
  font-weight:bold;
  cursor:pointer;
  margin-top:20px;
}
@keyframes fadeIn{
  from{opacity:0}
  to{opacity:1}
}
.heart{
  position:fixed;
  color:#ff4d6d;
  font-size:24px;
  animation:fall 4s linear infinite;
}
@keyframes fall{
  0%{transform:translateY(-10vh);}
  100%{transform:translateY(110vh);}
}
</style>
</head>
<body>

<div id="giftScreen">
  <div class="gift-box" onclick="openGift()">🎁</div>
  <p>Klik kotak hadiahnya 🎁</p>
</div>

<div id="letter" style="display:none;">
  <iframe style="border-radius:12px"
    src="https://www.youtube.com/embed/kEXAMPLE?autoplay=1&loop=1"
    width="300"
    height="80"
    frameborder="0"
    allow="autoplay; encrypted-media">
  </iframe>
  <p id="text">
farah...  

akhir" ini aku sadar kalau aku kurang menghargai ko,  
padahal ko itu luar biasa, perhatian ko itu bukan hal kecil  
aku minta maaf kalau aku bikin ko ngerasa kurang dihargai  
dan aku mau berubah, jadi versi yang lebih baik  
aku harap ko masih mau di sini 💖
  </p>
  <button onclick="love()">maafin aku?</button>
</div>

<script>
function openGift(){
  document.getElementById("giftScreen").style.display="none";
  document.getElementById("letter").style.display="block";
}

function love(){
  for(let i=0;i<20;i++){
    let heart=document.createElement("div");
    heart.className="heart";
    heart.style.left=Math.random()*100+"vw";
    heart.innerHTML="❤️";
    document.body.appendChild(heart);
  }
}
</script>

</body>
</html>
