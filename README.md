# Cantinho-lunar-
Site para minha loja 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Almanaque Pagão Anual | Cantinho Lunar</title>

<style>
:root{
  --ouro:#e6c76a;
  --roxo:#2b103a;
  --preto:#0b0614;
}
body{
  margin:0;
  background:
    radial-gradient(circle at top, #2d1240 0%, #0b0614 60%);
  color:#f5ecd1;
  font-family:Georgia, serif;
}
.container{
  max-width:1200px;
  margin:auto;
  padding:40px 25px;
}
header{
  text-align:center;
  margin-bottom:60px;
}
header h1{
  font-size:42px;
  color:var(--ouro);
  letter-spacing:1px;
}
header p{
  opacity:.85;
  font-style:italic;
}
.luna{
  width:120px;
  height:120px;
  border-radius:50%;
  background:
    radial-gradient(circle at 30% 30%, #fff8dc, #d4b65f);
  box-shadow:0 0 40px rgba(230,199,106,.6);
  margin:30px auto;
}
.month{
  margin-bottom:100px;
}
.month h2{
  text-align:center;
  color:var(--ouro);
  border-bottom:1px solid rgba(230,199,106,.4);
  padding-bottom:10px;
}
.subtitle{
  text-align:center;
  opacity:.8;
  margin:15px 0 30px;
}
table{
  width:100%;
  border-collapse:collapse;
}
th,td{
  border:1px solid rgba(255,255,255,.1);
  padding:8px;
  text-align:center;
}
th{
  background:rgba(255,255,255,.05);
}
.day-btn{
  background:rgba(0,0,0,.4);
  border:1px solid var(--ouro);
  color:var(--ouro);
  padding:6px 12px;
  border-radius:30px;
  cursor:pointer;
  font-size:14px;
}
.day-btn:hover{
  background:var(--ouro);
  color:#0b0614;
}
.info{
  display:none;
  background:
    linear-gradient(145deg, rgba(0,0,0,.7), rgba(30,10,40,.9));
  border:1px solid rgba(230,199,106,.4);
  padding:25px;
  border-radius:20px;
  margin-top:25px;
}
.info h3{
  margin-top:0;
  color:var(--ouro);
}
.prompt{
  margin-top:15px;
  background:rgba(255,255,255,.05);
  padding:15px;
  border-radius:12px;
  font-size:14px;
}
footer{
  text-align:center;
  margin-top:80px;
  opacity:.7;
  font-size:14px;
}
@media(max-width:600px){
  header h1{font-size:32px;}
}
</style>

<script>
function numerologia(d){
  let s=d.toString().split('').reduce((a,b)=>a+Number(b),0);
  while(s>9){s=s.toString().split('').reduce((a,b)=>a+Number(b),0);}
  return s;
}
function abrir(id){
  document.querySelectorAll('.info').forEach(e=>e.style.display='none');
  document.getElementById(id).style.display='block';
  document.getElementById(id).scrollIntoView({behavior:'smooth'});
}
</script>
</head>

<body>
<div class="container">

<header>
  <h1>Almanaque Pagão Anual</h1>
  <div class="luna"></div>
  <p>Cantinho Lunar • Deuses • Ciclos • Magia Natural</p>
</header>

<!-- JANEIRO -->
<div class="month">
<h2>Janeiro</h2>
<p class="subtitle">Renovação • Portais • Estrutura espiritual</p>

<table>
<tr><th>DOM</th><th>SEG</th><th>TER</th><th>QUA</th><th>QUI</th><th>SEX</th><th>SÁB</th></tr>
<tr>
<td></td>
<td><button class="day-btn" onclick="abrir('jan1')">1</button></td>
<td><button class="day-btn" onclick="abrir('jan2')">2</button></td>
<td>3</td><td>4</td><td>5</td><td>6</td>
</tr>
</table>

<div id="jan1" class="info">
<h3>🌑 Deusa Tripla & Janus</h3>
<b>Numerologia:</b> <script>document.write(numerologia(1))</script><br><br>
Inícios, passagens, abertura de caminhos.
<div class="prompt">
PROMPT IA:<br>
Deusa Tripla e Deus Janus,
lua nova dourada, paganismo europeu,
arte mística ritualística,
tons roxo profundo e ouro,
pintura digital realista sagrada
</div>
</div>

<div id="jan2" class="info">
<h3>Inana — Céu e Terra</h3>
<b>Numerologia:</b> <script>document.write(numerologia(2))</script><br><br>
Fertilidade, equilíbrio e polaridade.
<div class="prompt">
PROMPT IA:<br>
Deusa Inana mesopotâmica,
símbolos sumérios antigos,
estrelas cósmicas,
arte mística ancestral,
tons azul noturno e dourado
</div>
</div>
</div>

<footer>
🌙 Almanaque Pagão • Cantinho Lunar • Sabedoria Ancestral
</footer>

</div>
</body>
</html>
