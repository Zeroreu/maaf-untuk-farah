<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>untuk ko 🌸</title>
<style>
body{
  margin:0;
  overflow:hidden;
  height:100vh;
  background: linear-gradient(to top, #ff9a9e, #fad0c4);
  display:flex;
  justify-content:center;
  align-items:center;
  font-family: 'Poppins', sans-serif;
  color:white;
  text-align:center;
}

h1{
  font-size:28px;
  z-index:2;
  pointer-events:none;
}

.flower{
  position:fixed;
  top:-10px;
  font-size:24px;
  animation: fall linear infinite;
}

@keyframes fall{
  0%{
    transform: translateY(-10vh) rotate(0deg);
    opacity:1;
  }
  100%{
    transform: translateY(110vh) rotate(360deg);
    opacity:0;
  }
}
</style>
</head>

<body>

<h1>🌸 untuk ko 🌸</h1>

<!-- lagu Bersenja Gurau -->
<iframe width="0" height="0"
src="https://www.youtube.com/embed/jmvX6XyvCy0?autoplay=1&loop=1&playlist=jmvX6XyvCy0"
frameborder="0"
allow="autoplay">
</iframe>

<script>
function createFlower(){
  const flower=document.createElement("div");
  flower.className="flower";

  const flowers=["🌸","🌷","💮","🌺"];
  flower.innerHTML=flowers[Math.floor(Math.random()*flowers.length)];

  flower.style.left=Math.random()*100+"vw";
  flower.style.animationDuration=(3+Math.random()*5)+"s";

  document.body.appendChild(flower);

  setTimeout(()=>{
    flower.remove();
  },8000);
}

setInterval(createFlower,400);
</script>

</body>
</html>
