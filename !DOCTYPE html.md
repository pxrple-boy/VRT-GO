<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>VRT!GO — experience CBD</title>  
  
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Bebas+Neue&display=swap" rel="stylesheet">  
  
<style>  
:root {  
  --neon: #39FF14;  
  --black: #0B0B0B;  
  --dark: #111;  
}  
  
* { margin:0; padding:0; box-sizing:border-box; }  
  
body {  
  background: var(--black);  
  color: var(--neon);  
  font-family: 'Space Mono', monospace;  
  overflow-x: hidden;  
}  
  
/* scanlines */  
body::before {  
  content:'';  
  position:fixed;  
  inset:0;  
  background: repeating-linear-gradient(  
    0deg,  
    transparent,  
    transparent 2px,  
    rgba(0,0,0,0.06) 2px,  
    rgba(0,0,0,0.06) 4px  
  );  
  pointer-events:none;  
}  
  
/* HERO */  
.hero {  
  height:100vh;  
  display:flex;  
  flex-direction:column;  
  justify-content:center;  
  align-items:center;  
  text-align:center;  
}  
  
.hero h1 {  
  font-family:'Bebas Neue', sans-serif;  
  font-size:5rem;  
  letter-spacing:4px;  
  text-shadow:0 0 20px var(--neon);  
}  
  
.hero p {  
  margin-top:20px;  
  opacity:0.7;  
}  
  
/* BUTTON */  
.btn {  
  margin-top:30px;  
  padding:12px 30px;  
  border:1px solid var(--neon);  
  background:transparent;  
  color:var(--neon);  
  cursor:pointer;  
  transition:0.2s;  
}  
  
.btn:hover {  
  background:var(--neon);  
  color:black;  
  box-shadow:0 0 20px var(--neon);  
}  
  
/* SECTIONS */  
section {  
  padding:80px 20px;  
  text-align:center;  
}  
  
.grid {  
  display:grid;  
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));  
  gap:20px;  
  margin-top:40px;  
}  
  
.card {  
  border:1px solid #222;  
  padding:20px;  
  background: #111;  
  transition:0.2s;  
}  
  
.card:hover {  
  border-color:var(--neon);  
  transform:translateY(-5px);  
}  
  
/* FOOTER */  
footer {  
  padding:40px;  
  text-align:center;  
  font-size:0.8rem;  
  opacity:0.5;  
}  
</style>  
</head>  
  
<body>  
  
<div class="hero">  
  <h1>VRT!GO</h1>  
  <p>ENTER THE CBD EXPERIENCE</p>  
  <button class="btn" onclick="scrollToSection()">ENTER</button>  
</div>  
  
<section id="experience">  
  <h2>EXPERIENCE</h2>  
  <p>Une nouvelle perception. Une nouvelle fréquence.</p>  
  
  <div class="grid">  
    <div class="card">FLOW</div>  
    <div class="card">RELAX</div>  
    <div class="card">BOOST</div>  
  </div>  
</section>  
  
<section>  
  <h2>PRODUCTS</h2>  
  <div class="grid">  
    <div class="card">VRT!GO Oil</div>  
    <div class="card">VRT!GO Vape</div>  
    <div class="card">VRT!GO Gummies</div>  
  </div>  
</section>  
  
<section>  
  <h2>CONTACT</h2>  
  <p>vrtigo.contact@mail.com</p>  
</section>  
  
<footer>  
  © VRT!GO — 2026  
</footer>  
  
<script>  
function scrollToSection() {  
  document.getElementById("experience").scrollIntoView({  
    behavior: "smooth"  
  });  
}  
</script>  
  
</body>  
</html>  
