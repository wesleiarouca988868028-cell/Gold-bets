# Gold
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>GolDeBets – Apostas com as Melhores Odds do Brasil</title>
  <meta name="description" content="Cadastre-se, ganhe bônus de R$ 300 e receba seu Pix em 10 min. Odds atualizadas ao vivo." />

  <!-- Favicon Bandeira do Brasil (SVG inline) -->
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,
  <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'>
    <rect width='512' height='512' fill='%2300963f'/>
    <polygon points='256,60 460,256 256,452 52,256' fill='%23ffdf00'/>
    <circle cx='256' cy='256' r='90' fill='%23002776'/>
  </svg>"/>

  <style>
    :root{
      --bg:#0d1117;
      --bg2:#161b22;
      --accent:#1fdf64;
      --text:#e6edf3;
      --muted:#9ba3af;
      --card:#1c2128;
    }
    *{box-sizing:border-box;margin:0;padding:0}
    body{
      font-family:Inter,system-ui,Arial;
      background:var(--bg);
      color:var(--text);
      line-height:1.6;
    }
    a{color:inherit;text-decoration:none}
    header{
      position:fixed;top:0;left:0;right:0;
      background:rgba(13,17,23,.95);
      backdrop-filter:blur(8px);
      border-bottom:1px solid #222;
      z-index:1000;
    }
    .container{max-width:1200px;margin:auto;padding:0 20px}
    .nav{
      display:flex;align-items:center;justify-content:space-between;
      height:64px;
    }
    .logo{
      font-weight:900;font-size:1.4rem;color:var(--accent);
    }
    nav a{
      margin-left:18px;font-weight:500;color:var(--muted)
    }
    nav a:hover{color:var(--text)}

    main{padding-top:90px}

    .hero{
      padding:80px 0;
      background:linear-gradient(135deg,#0d1117,#0b1f13);
      text-align:center;
    }
    .hero h1{
      font-size:clamp(2rem,4vw,3.2rem);
      margin-bottom:12px;
    }
    .hero p{color:var(--muted);max-width:720px;margin:0 auto 28px}
    .btn{
      background:var(--accent);
      color:#000;
      padding:14px 28px;
      border-radius:8px;
      font-weight:700;
      display:inline-block;
    }

    section{padding:70px 0}
    h2{margin-bottom:30px;font-size:1.9rem}

    .odds-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:18px;
    }
    .odd-card{
      background:var(--card);
      border-radius:10px;
      padding:16px;
    }
    .odd-card h3{font-size:1rem;margin-bottom:8px}
    .odd{
      display:flex;justify-content:space-between;
      margin-top:6px;font-weight:600;
    }
    .odd span:last-child{color:var(--accent)}

    .steps{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
      gap:24px;
      text-align:center;
    }
    .step{
      background:var(--card);
      padding:28px;
      border-radius:12px;
    }
    .step .icon{font-size:2.2rem;margin-bottom:10px}

    table{
      width:100%;
      border-collapse:collapse;
      background:var(--card);
      border-radius:12px;
      overflow:hidden;
    }
    th,td{padding:16px;text-align:left}
    th{background:#222}
    tr:not(:last-child){border-bottom:1px solid #2a2f36}

    .testimonials{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
      gap:20px;
    }
    .testimonial{
      background:var(--card);
      padding:22px;
      border-radius:12px;
    }
    .stars{color:#ffd000}

    .faq details{
      background:var(--card);
      border-radius:10px;
      padding:16px;
      margin-bottom:12px;
    }
    .faq summary{cursor:pointer;font-weight:600}

    footer{
      background:#020409;
      padding:40px 0;
      color:var(--muted);
      font-size:.9rem;
    }
    footer .container{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:20px;
    }
    .badge18{
      font-size:1.4rem;font-weight:900;color:#fff
    }

    @media(max-width:600px){
      nav{display:none}
    }
  </style>
</head>

<body>
<header>
  <div class="container nav">
    <div class="logo">GolDeBets</div>
    <nav>
      <a href="#">Ao Vivo</a>
      <a href="#">Hoje</a>
      <a href="#">Amanhã</a>
      <a href="#">Promos</a>
      <a href="#">App</a>
    </nav>
  </div>
</header>

<main>
  <section class="hero">
    <div class="container">
      <h1>Odds Maiores que a da Várzea</h1>
      <p>Pix de R$ 1, saque em 10 min, bônus 150 % até R$ 300</p>
      <a class="btn" href="#cadastro" id="btnCadastro">Cadastrar com CPF</a>
    </div>
  </section>

  <section>
    <div class="container">
      <h2>🔥 Odds ao Vivo</h2>
      <div class="odds-grid" id="odds">
        <!-- JS -->
      </div>
    </div>
  </section>

  <section>
    <div class="container">
      <h2>Como Apostar em 3 Passos</h2>
      <div class="steps">
        <div class="step"><div class="icon">📝</div><strong>Cadastro 30 s</strong></div>
        <div class="step"><div class="icon">⚡</div><strong>Depósito Pix R$ 1</strong></div>
        <div class="step"><div class="icon">🎯</div><strong>Clique na odd e aposte</strong></div>
      </div>
    </div>
  </section>

  <section>
    <div class="container">
      <h2>Comparativo de Retorno</h2>
      <table>
        <tr><th>Plataforma</th><th>ROI / RTP</th><th>Fonte</th></tr>
        <tr><td><strong>GolDeBets</strong></td><td>94,2 %</td><td>RTP real</td></tr>
        <tr><td>Média Mercado</td><td>92 %</td><td>Relatório IBIA 2026</td></tr>
      </table>
    </div>
  </section>

  <section>
    <div class="container">
      <h2>O que a galera fala</h2>
      <div class="testimonials">
        <div class="testimonial">
          <div class="stars">★★★★☆</div>
          “Saquei R$ 450 em 8 min”<br><small>— Carlos M.</small>
        </div>
        <div class="testimonial">
          <div class="stars">★★★★☆</div>
          “Odds maiores que na Betano”<br><small>— Rafael S.</small>
        </div>
        <div class="testimonial">
          <div class="stars">★★★★☆</div>
          “Pix caiu mais rápido que gol do Flamengo”<br><small>— Bruno A.</small>
        </div>
      </div>
    </div>
  </section>

  <section class="faq">
    <div class="container">
      <h2>FAQ</h2>
      <details><summary>Pago imposto?</summary>Ganhos seguem legislação vigente.</details>
      <details><summary>Quais limites?</summary>Depósitos a partir de R$ 1.</details>
      <details><summary>Tem cash out?</summary>Sim, em eventos elegíveis.</details>
      <details><summary>É seguro?</summary>Criptografia SSL e KYC.</details>
      <details><summary>Regras FIFA?</summary>Eventos oficiais regulamentados.</details>
    </div>
  </section>
</main>

<footer>
  <div class="container">
    <div>
      <div class="badge18">18+</div>
      Jogue com responsabilidade
    </div>
    <div>
      Licença MF/SPA sob consulta<br/>
      SELIC • Brasil
    </div>
    <div>
      Política de Cookies<br/>
      Jogo Responsável
    </div>
  </div>
</footer>

<script>
const jogos = [
  {liga:"Libertadores", jogo:"Palmeiras x Flamengo", a:1.83, e:3.60, b:3.40},
  {liga:"Brasileirão", jogo:"Grêmio x Inter", a:2.10, e:3.20, b:3.10},
  {liga:"Brasileirão", jogo:"Corinthians x Santos", a:1.95, e:3.30, b:3.80},
  {liga:"NBA", jogo:"Lakers x Celtics", a:1.72, b:2.10},
  {liga:"NBA", jogo:"Heat x Bulls", a:1.88, b:1.98}
];

function variar(v){
  return (v + (Math.random()*0.1 - 0.05)).toFixed(2);
}

function render(){
  const box = document.getElementById("odds");
  box.innerHTML="";
  jogos.forEach(j=>{
    box.innerHTML+=`
      <div class="odd-card">
        <h3>${j.liga}<br>${j.jogo}</h3>
        <div class="odd"><span>Casa</span><span>${variar(j.a)}</span></div>
        ${j.e?`<div class="odd"><span>Empate</span><span>${variar(j.e)}</span></div>`:""}
        <div class="odd"><span>Fora</span><span>${variar(j.b)}</span></div>
      </div>`;
  });
}
render();
setInterval(render,30000);

document.getElementById("btnCadastro").addEventListener("click",()=>{
  const cpf = prompt("Digite seu CPF para cadastro:");
  if(cpf) localStorage.setItem("gdb_cpf",cpf);
});
</script>
</body>
</html>
