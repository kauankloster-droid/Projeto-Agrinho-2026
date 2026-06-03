<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sustentabilidade no Campo e na Cidade</title>

<style>
:root{
    --verde:#2e8b57;
    --verde-claro:#56c271;
    --azul:#4db8ff;
    --escuro:#123524;
    --claro:#f5fff7;
    --branco:#ffffff;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
    font-family:'Segoe UI',sans-serif;
}

body{
    background:var(--claro);
    color:#333;
}

/* MENU */
header{
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;
    background:rgba(18,53,36,0.95);
    backdrop-filter:blur(10px);
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:15px 8%;
}

.logo{
    color:white;
    font-size:1.4rem;
    font-weight:bold;
}

nav ul{
    display:flex;
    list-style:none;
    gap:20px;
}

nav a{
    text-decoration:none;
    color:white;
    transition:.3s;
}

nav a:hover{
    color:var(--verde-claro);
}

/* HERO */
.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    color:white;
    padding:100px 20px;
    background:
    linear-gradient(rgba(0,0,0,.45),rgba(0,0,0,.45)),
    url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1400&q=80');
    background-size:cover;
    background-position:center;
}

.hero-content{
    max-width:800px;
}

.hero h1{
    font-size:3rem;
    margin-bottom:20px;
}

.hero p{
    font-size:1.2rem;
    margin-bottom:25px;
}

.btn{
    background:var(--verde-claro);
    color:white;
    border:none;
    padding:15px 30px;
    border-radius:40px;
    cursor:pointer;
    font-size:1rem;
    transition:.3s;
}

.btn:hover{
    transform:translateY(-4px) scale(1.05);
    background:#3bb35a;
}

/* SEÇÕES */
section{
    padding:90px 8%;
}

.titulo{
    text-align:center;
    margin-bottom:50px;
}

.titulo h2{
    color:var(--escuro);
    font-size:2.2rem;
}

.titulo p{
    margin-top:10px;
}

/* CARDS */
.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
    gap:25px;
}

.card{
    background:white;
    padding:25px;
    border-radius:20px;
    box-shadow:0 10px 20px rgba(0,0,0,.08);
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 20px 30px rgba(0,0,0,.15);
}

.card h3{
    color:var(--verde);
    margin-bottom:10px;
}

/* CAMPO E CIDADE */
.duas-colunas{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:30px;
}

.bloco{
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 10px 20px rgba(0,0,0,.08);
}

.bloco:hover{
    transform:scale(1.02);
    transition:.3s;
}

.bloco h3{
    color:var(--verde);
    margin-bottom:15px;
}

/* CONTADOR */
.contador{
    background:linear-gradient(135deg,var(--verde),var(--azul));
    color:white;
    text-align:center;
    border-radius:25px;
    padding:50px 20px;
}

.numero{
    font-size:4rem;
    font-weight:bold;
}

/* QUIZ */
.quiz{
    background:white;
    border-radius:20px;
    padding:30px;
    max-width:700px;
    margin:auto;
    box-shadow:0 10px 20px rgba(0,0,0,.08);
}

.quiz button{
    margin-top:15px;
}

/* RODAPÉ */
footer{
    background:var(--escuro);
    color:white;
    text-align:center;
    padding:25px;
}

/* RESPONSIVO */
@media(max-width:768px){

    nav{
        flex-direction:column;
        gap:10px;
    }

    nav ul{
        flex-wrap:wrap;
        justify-content:center;
    }

    .hero h1{
        font-size:2.2rem;
    }

    .numero{
        font-size:3rem;
    }
}
</style>
</head>
<body>

<header>
<nav>
<div class="logo">🌱 EcoConexão</div>

<ul>
<li><a href="#inicio">Início</a></li>
<li><a href="#informacoes">Informações</a></li>
<li><a href="#campoCidade">Campo & Cidade</a></li>
<li><a href="#contador">Impacto</a></li>
<li><a href="#quiz">Quiz</a></li>
</ul>
</nav>
</header>

<section class="hero" id="inicio">
<div class="hero-content">
<h1>Sustentabilidade no Campo e na Cidade</h1>

<p>
O futuro depende das escolhas que fazemos hoje. Pequenas atitudes,
tanto no campo quanto na cidade, ajudam a preservar recursos naturais,
reduzir desperdícios e construir comunidades mais equilibradas.
</p>

<button class="btn" onclick="mostrarMensagem()">
Descobrir uma ação sustentável
</button>

<p id="mensagem" style="margin-top:20px;font-weight:bold;"></p>

</div>
</section>

<section id="informacoes">

<div class="titulo">
<h2>Pequenas ações, grandes resultados</h2>
<p>Conheça atitudes que contribuem para um planeta mais saudável.</p>
</div>

<div class="cards">

<div class="card">
<h3>♻️ Reciclagem</h3>
<p>
Separar materiais recicláveis reduz a quantidade de lixo enviada aos
aterros e permite o reaproveitamento de recursos.
</p>
</div>

<div class="card">
<h3>💧 Economia de Água</h3>
<p>
Fechar torneiras, reutilizar água quando possível e evitar desperdícios
preserva um recurso essencial para a vida.
</p>
</div>

<div class="card">
<h3>☀️ Energia Limpa</h3>
<p>
Fontes renováveis como solar e eólica ajudam a diminuir a emissão de
poluentes e tornam a produção de energia mais sustentável.
</p>
</div>

<div class="card">
<h3>🌳 Preservação Ambiental</h3>
<p>
Plantar árvores e proteger áreas verdes melhora a qualidade do ar,
favorece a biodiversidade e reduz o aquecimento local.
</p>
</div>

</div>
</section>

<section id="campoCidade">

<div class="titulo">
<h2>Campo e Cidade trabalhando juntos</h2>
<p>O equilíbrio ambiental depende da colaboração entre diferentes espaços.</p>
</div>

<div class="duas-colunas">

<div class="bloco">
<h3>🚜 Sustentabilidade no Campo</h3>

<p>
No meio rural, práticas como preservação do solo, uso racional da água,
rotação de culturas e proteção das nascentes contribuem para uma produção
mais eficiente e responsável.
</p>

<br>

<p>
Quando produtores adotam métodos sustentáveis, toda a sociedade se
beneficia com alimentos de qualidade e menor impacto ambiental.
</p>
</div>

<div class="bloco">
<h3>🏙️ Sustentabilidade na Cidade</h3>

<p>
Nas áreas urbanas, o descarte correto de resíduos, o uso de transporte
coletivo, a arborização e o consumo consciente ajudam a reduzir a pressão
sobre os recursos naturais.
</p>

<br>

<p>
Cada cidadão pode contribuir tornando sua rotina mais equilibrada e
respeitosa com o meio ambiente.
</p>
</div>

</div>

</section>

<section>

<div class="duas-colunas">

<div class="bloco">
<h3>♻️ Reciclagem Inteligente</h3>
<p>
A reciclagem transforma materiais que seriam descartados em novos produtos.
Além de reduzir o lixo, ela economiza matéria-prima e energia.
</p>
</div>

<div class="bloco">
<h3>💡 Energia Limpa para o Futuro</h3>
<p>
A expansão das energias renováveis representa uma alternativa importante
para diminuir impactos ambientais e fortalecer o desenvolvimento sustentável.
</p>
</div>

</div>

</section>

<section id="contador">

<div class="contador">

<h2>Atitudes sustentáveis registradas</h2>

<div class="numero" id="numero">0</div>

<p>
Cada pequena ação conta para construir um futuro melhor.
</p>

</div>

</section>

<section id="quiz">

<div class="titulo">
<h2>Quiz Sustentável</h2>
<p>Teste seus conhecimentos.</p>
</div>

<div class="quiz">

<h3>
Qual atitude ajuda a economizar água?
</h3>

<br>

<input type="radio" name="resposta" value="errado">
Deixar a torneira aberta ao escovar os dentes

<br><br>

<input type="radio" name="resposta" value="certo">
Fechar a torneira durante a escovação

<br><br>

<input type="radio" name="resposta" value="errado">
Lavar calçadas diariamente

<br>

<button class="btn" onclick="verificarQuiz()">
Verificar Resposta
</button>

<p id="resultadoQuiz" style="margin-top:20px;font-weight:bold;"></p>

</div>

</section>

<footer>
<h3>🌱 Projeto Agrinho 2026</h3>
<p>Sustentabilidade no Campo e na Cidade</p>
</footer>

<script>

// BOTÃO INTERATIVO
function mostrarMensagem(){

const dicas = [
"🌿 Plante uma árvore e ajude a melhorar a qualidade do ar.",
"💧 Reduza o tempo no banho para economizar água.",
"♻️ Separe resíduos recicláveis corretamente.",
"🚲 Utilize bicicleta ou caminhe em pequenos trajetos.",
"☀️ Aproveite a luz natural sempre que possível."
];

const aleatoria =
dicas[Math.floor(Math.random()*dicas.length)];

document.getElementById("mensagem").innerText = aleatoria;
}

// CONTADOR ANIMADO
let contador = 0;
const alvo = 2026;

const animacao = setInterval(() => {
contador += 13;

if(contador >= alvo){
contador = alvo;
clearInterval(animacao);
}

document.getElementById("numero").innerText = contador;

}, 20);

// QUIZ
function verificarQuiz(){

const resposta =
document.querySelector('input[name="resposta"]:checked');

const resultado =
document.getElementById("resultadoQuiz");

if(!resposta){
resultado.innerHTML = "⚠️ Escolha uma alternativa.";
return;
}

if(resposta.value === "certo"){
resultado.innerHTML =
"✅ Muito bem! Essa atitude ajuda a preservar água.";
}
else{
resultado.innerHTML =
"❌ Tente novamente. Pense em como evitar desperdícios.";
}
}

</script>

</body>
</html>
