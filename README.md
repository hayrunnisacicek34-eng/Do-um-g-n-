<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>İyi ki Doğdun Yağmur 💗</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&family=Pacifico&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
font-family:Poppins,sans-serif;
background:linear-gradient(135deg,#fff0f7,#ffe4f1,#ffd6ea);
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
color:#ff4d94;
text-align:center;
}
.card{
background:rgba(255,255,255,.55);
backdrop-filter:blur(15px);
padding:40px;
border-radius:30px;
width:90%;
max-width:700px;
box-shadow:0 15px 40px rgba(255,105,180,.25);
animation:fade 1.5s;
}
h1{
font-family:Pacifico;
font-size:58px;
margin-bottom:15px;
}
p{
font-size:18px;
line-height:1.9;
}
button{
margin-top:25px;
padding:14px 35px;
border:none;
border-radius:40px;
background:#ff6aa8;
color:#fff;
font-size:18px;
cursor:pointer;
transition:.3s;
}
button:hover{
transform:scale(1.08);
}
#letter{
display:none;
margin-top:25px;
animation:fade 1s;
}
.heart{
position:fixed;
bottom:-40px;
font-size:25px;
animation:fly linear infinite;
opacity:.7;
}
@keyframes fly{
0%{transform:translateY(0);}
100%{transform:translateY(-120vh);}
}
@keyframes fade{
from{opacity:0;transform:translateY(20px);}
to{opacity:1;transform:translateY(0);}
}
</style>
</head>

<body>

<div class="card">

<h1>🎂 Yağmur 💗</h1>

<p>
Bugün tam 19 yaşına girdin... 🌸<br><br>

Hayat bazen insanın karşısına öyle güzel insanlar çıkarıyor ki...
İşte sen benim için tam olarak öyle birisin. 🤍
</p>

<button onclick="showLetter()">
💌 Mektubu Aç
</button>

<div id="letter">

<p>

İyi ki varsın...

İyi ki hayatımdasın...

Umarım bu yeni yaşın sana bolca mutluluk, huzur, sağlık ve kahkaha getirir. 💕

Her zaman yüzünün gülmesini diliyorum.

Hayallerinin birer birer gerçekleştiği harika bir yaş olsun. ✨

<b>İYİ Kİ DOĞDUNN! 🎉</b>

<br><br>

🩷 <b>Seni çok seven Hayrun💗</b>

</p>

</div>

</div>

<script>

function showLetter(){
document.getElementById("letter").style.display="block";
}

for(let i=0;i<25;i++){
let h=document.createElement("div");
h.className="heart";
h.innerHTML=["💗","🩷","🌸","✨","💕"][Math.floor(Math.random()*5)];
h.style.left=Math.random()*100+"vw";
h.style.animationDuration=(6+Math.random()*6)+"s";
h.style.animationDelay=Math.random()*6+"s";
document.body.appendChild(h);
}

</script>

</body>
</html>
