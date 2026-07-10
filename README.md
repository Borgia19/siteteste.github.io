<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dra. Lohrane Sousa · Harmonização Facial & Corporal — Centro, Curitiba</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,500;0,9..144,600;1,9..144,500&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #FAF6F0;
    --bg-deep: #F2ECE2;
    --ink: #2A231D;
    --ink-soft: #6B5D52;
    --accent: #3F5C4C;
    --accent-dark: #2C4238;
    --accent-soft: #E9DFCF;
    --rose: #D9A9A0;
    --gold: #B08D57;
    --white: #FFFFFF;
    --line: rgba(42,35,29,0.12);
    --shadow: 0 20px 50px -25px rgba(42,35,29,0.35);
    --radius-blob: 62% 38% 55% 45% / 45% 55% 45% 55%;
  }

  *{ box-sizing:border-box; }
  html{ scroll-behavior:smooth; }
  body{
    margin:0;
    background:var(--bg);
    color:var(--ink);
    font-family:'Manrope', sans-serif;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  h1,h2,h3, .display{
    font-family:'Fraunces', serif;
    font-weight:500;
    letter-spacing:-0.01em;
    line-height:1.05;
    margin:0;
  }
  p{ margin:0; }
  a{ color:inherit; text-decoration:none; }
  img{ max-width:100%; display:block; }
  ul{ margin:0; padding:0; list-style:none; }
  section{ position:relative; }

  .wrap{
    max-width:1180px;
    margin:0 auto;
    padding:0 32px;
  }

  @media (prefers-reduced-motion: reduce){
    *{ animation:none !important; transition:none !important; }
  }

  /* ---------- Nav ---------- */
  header{
    position:sticky; top:0; z-index:50;
    background:rgba(250,246,240,0.86);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--line);
  }
  .nav{
    display:flex; align-items:center; justify-content:space-between;
    padding:18px 32px;
    max-width:1180px; margin:0 auto;
  }
  .brand{
    font-family:'Fraunces', serif;
    font-size:20px;
    font-style:italic;
    font-weight:500;
    display:flex; align-items:center; gap:10px;
  }
  .brand-dot{
    width:8px; height:8px; border-radius:50%;
    background:var(--rose);
    display:inline-block;
  }
  .nav-links{
    display:flex; align-items:center; gap:36px;
    font-size:14px; color:var(--ink-soft);
  }
  .nav-links a:hover{ color:var(--accent); }
  .btn{
    display:inline-flex; align-items:center; gap:8px;
    padding:13px 26px;
    background:var(--accent);
    color:var(--white);
    border-radius:999px;
    font-size:14px; font-weight:700;
    letter-spacing:0.01em;
    box-shadow:0 12px 24px -10px rgba(63,92,76,0.55);
    transition:transform .25s ease, box-shadow .25s ease, background .25s ease;
    white-space:nowrap;
  }
  .btn:hover{ transform:translateY(-2px); background:var(--accent-dark); box-shadow:0 16px 30px -10px rgba(63,92,76,0.6); }
  .btn:focus-visible, a:focus-visible, button:focus-visible{
    outline:2px solid var(--gold); outline-offset:3px;
  }
  .btn-ghost{
    background:transparent; color:var(--ink);
    border:1.5px solid var(--line);
    box-shadow:none;
  }
  .btn-ghost:hover{ background:var(--white); transform:none; border-color:var(--accent); }
  .nav .btn{ padding:11px 22px; font-size:13.5px; }

  /* ---------- Hero ---------- */
  .hero{
    padding:76px 0 40px;
    overflow:hidden;
  }
  .hero-grid{
    display:grid;
    grid-template-columns:1.05fr 0.95fr;
    gap:64px;
    align-items:center;
  }
  .eyebrow{
    font-size:12.5px;
    letter-spacing:0.14em;
    text-transform:uppercase;
    color:var(--accent);
    font-weight:700;
    display:flex; align-items:center; gap:10px;
    margin-bottom:22px;
  }
  .eyebrow::before{
    content:''; width:26px; height:1.5px; background:var(--gold);
  }
  .hero h1{
    font-size:clamp(38px, 4.6vw, 60px);
    color:var(--ink);
  }
  .hero h1 em{
    font-style:italic; color:var(--accent);
  }
  .hero-sub{
    margin-top:24px;
    font-size:18px;
    line-height:1.6;
    color:var(--ink-soft);
    max-width:480px;
  }
  .hero-ctas{
    margin-top:36px;
    display:flex; align-items:center; gap:18px; flex-wrap:wrap;
  }
  .hero-ctas .btn{ padding:17px 32px; font-size:15px; }

  .rating-inline{
    margin-top:34px;
    display:flex; align-items:center; gap:14px;
  }
  .stars{ color:var(--gold); font-size:16px; letter-spacing:2px; }
  .rating-inline .num{ font-family:'Fraunces', serif; font-size:20px; font-weight:600; }
  .rating-inline .cap{ font-size:13px; color:var(--ink-soft); }

  /* Hero visual */
  .hero-visual{
    position:relative;
    height:520px;
  }
  .blob{
    position:absolute;
    border-radius:var(--radius-blob);
  }
  .blob-1{
    width:88%; height:88%;
    top:0; left:6%;
    background:linear-gradient(150deg, var(--accent-soft), #fff 70%);
    border:1px solid var(--line);
  }
  .blob-2{
    width:58%; height:58%;
    bottom:-6%; right:-4%;
    background:linear-gradient(140deg, var(--rose), #efc9c1);
    opacity:0.55;
    animation:float 9s ease-in-out infinite;
  }
  @keyframes float{
    0%,100%{ transform:translate(0,0) rotate(0deg); }
    50%{ transform:translate(-10px, 14px) rotate(6deg); }
  }
  .card-float{
    position:absolute;
    background:var(--white);
    border-radius:20px;
    box-shadow:var(--shadow);
    padding:20px 22px;
    display:flex; align-items:center; gap:14px;
  }
  .card-float.rating{
    top:12%; left:-2%;
    animation:floatSmall 6s ease-in-out infinite;
  }
  .card-float.since{
    bottom:10%; left:12%;
    animation:floatSmall 7s ease-in-out infinite reverse;
  }
  @keyframes floatSmall{
    0%,100%{ transform:translateY(0); }
    50%{ transform:translateY(-10px); }
  }
  .card-float .icon-circle{
    width:44px; height:44px; border-radius:50%;
    background:var(--accent-soft);
    display:flex; align-items:center; justify-content:center;
    font-size:20px;
  }
  .card-float .t1{ font-weight:800; font-size:15px; }
  .card-float .t2{ font-size:12.5px; color:var(--ink-soft); }

  /* ---------- Social proof strip ---------- */
  .proof{
    background:var(--accent-dark);
    color:#fff;
    padding:26px 0;
  }
  .proof .wrap{
    display:flex; align-items:center; justify-content:center; gap:60px;
    flex-wrap:wrap;
  }
  .proof-item{ display:flex; align-items:center; gap:12px; font-size:14.5px; }
  .proof-item strong{ font-family:'Fraunces', serif; font-size:19px; font-weight:600; }
  .proof-divider{ width:1px; height:22px; background:rgba(255,255,255,0.22); }

  /* ---------- Section heading ---------- */
  .section-head{
    max-width:640px;
    margin:0 auto 56px;
    text-align:center;
  }
  .section-head .eyebrow{ justify-content:center; }
  .section-head .eyebrow::before{ display:none; }
  .section-head h2{
    font-size:clamp(30px, 3.4vw, 42px);
    margin-top:14px;
  }
  .section-head p{
    margin-top:16px;
    color:var(--ink-soft);
    font-size:16px;
    line-height:1.6;
  }

  /* ---------- Services ---------- */
  .services{ padding:110px 0 100px; }
  .service-grid{
    display:grid;
    grid-template-columns:repeat(3, 1fr);
    gap:26px;
  }
  .service-card{
    background:var(--white);
    border:1px solid var(--line);
    border-radius:24px;
    padding:34px 28px;
    transition:transform .3s ease, box-shadow .3s ease, border-color .3s ease;
  }
  .service-card:hover{
    transform:translateY(-6px);
    box-shadow:var(--shadow);
    border-color:transparent;
  }
  .service-petal{
    width:52px; height:52px;
    border-radius:var(--radius-blob);
    background:var(--accent-soft);
    display:flex; align-items:center; justify-content:center;
    font-size:22px;
    margin-bottom:22px;
  }
  .service-card h3{
    font-size:20px; font-weight:600; margin-bottom:10px;
  }
  .service-card p{
    font-size:14.5px; line-height:1.6; color:var(--ink-soft);
  }

  /* ---------- Process ---------- */
  .process{
    background:var(--bg-deep);
    padding:100px 0;
  }
  .process-row{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:0;
    position:relative;
  }
  .process-row::before{
    content:'';
    position:absolute;
    top:26px; left:16.6%; right:16.6%;
    height:1px;
    background:repeating-linear-gradient(to right, var(--gold) 0 8px, transparent 8px 16px);
  }
  .process-step{ text-align:center; padding:0 20px; }
  .process-num{
    width:52px; height:52px; margin:0 auto 24px;
    border-radius:50%;
    background:var(--accent);
    color:#fff;
    font-family:'Fraunces', serif;
    display:flex; align-items:center; justify-content:center;
    font-size:19px;
    position:relative; z-index:2;
    box-shadow:0 10px 22px -8px rgba(63,92,76,0.5);
  }
  .process-step h3{ font-size:18px; font-weight:600; margin-bottom:10px; }
  .process-step p{ font-size:14.5px; color:var(--ink-soft); line-height:1.6; max-width:260px; margin:0 auto; }

  /* ---------- About ---------- */
  .about{
    padding:110px 0;
  }
  .about-grid{
    display:grid;
    grid-template-columns:0.85fr 1.15fr;
    gap:70px;
    align-items:center;
  }
  .about-visual{
    position:relative;
    height:420px;
  }
  .about-blob{
    position:absolute; inset:0;
    border-radius:var(--radius-blob);
    background:linear-gradient(160deg, var(--rose), var(--accent-soft) 65%);
    display:flex; align-items:center; justify-content:center;
  }
  .about-blob span{
    font-family:'Fraunces', serif;
    font-style:italic;
    font-size:22px;
    color:var(--accent-dark);
    text-align:center;
    padding:0 40px;
  }
  .quotes{
    margin-top:34px;
    display:flex; flex-direction:column; gap:18px;
  }
  .quote{
    padding:18px 22px;
    background:var(--white);
    border-left:3px solid var(--gold);
    border-radius:0 14px 14px 0;
    font-size:14.5px;
    line-height:1.6;
    color:var(--ink);
  }
  .quote span{
    display:block; margin-top:8px;
    font-size:12.5px; color:var(--ink-soft); font-weight:700;
    letter-spacing:0.03em; text-transform:uppercase;
  }

  /* ---------- Location ---------- */
  .location{
    background:var(--accent-dark);
    color:#fff;
    padding:100px 0;
  }
  .loc-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
  }
  .location .eyebrow{ color:var(--rose); }
  .location h2{ font-size:clamp(28px,3.2vw,38px); color:#fff; }
  .loc-list{ margin-top:28px; display:flex; flex-direction:column; gap:20px; }
  .loc-item{ display:flex; gap:16px; align-items:flex-start; }
  .loc-icon{
    width:38px; height:38px; border-radius:50%;
    background:rgba(255,255,255,0.12);
    display:flex; align-items:center; justify-content:center;
    flex-shrink:0; font-size:16px;
  }
  .loc-item .t1{ font-weight:700; font-size:15px; }
  .loc-item .t2{ font-size:14px; color:rgba(255,255,255,0.72); margin-top:3px; line-height:1.5; }
  .loc-card{
    background:rgba(255,255,255,0.06);
    border:1px solid rgba(255,255,255,0.14);
    border-radius:24px;
    padding:40px;
  }
  .loc-card .status{
    display:inline-flex; align-items:center; gap:8px;
    background:rgba(255,255,255,0.1);
    padding:6px 14px; border-radius:999px;
    font-size:12.5px; font-weight:700;
    margin-bottom:22px;
  }
  .status-dot{ width:7px; height:7px; border-radius:50%; background:#8fce9f; }
  .loc-card h3{ font-size:22px; color:#fff; margin-bottom:8px; font-family:'Fraunces', serif; font-weight:500; }
  .loc-card p{ color:rgba(255,255,255,0.72); font-size:14.5px; line-height:1.6; }
  .loc-card .btn{ margin-top:26px; width:100%; justify-content:center; }

  /* ---------- Final CTA ---------- */
  .final-cta{
    padding:110px 0;
    text-align:center;
  }
  .final-cta h2{
    font-size:clamp(32px, 4vw, 50px);
    max-width:620px; margin:0 auto;
  }
  .final-cta p{
    margin-top:20px;
    color:var(--ink-soft);
    font-size:17px;
  }
  .final-cta .btn{
    margin-top:36px;
    padding:19px 40px;
    font-size:16px;
  }

  /* ---------- Footer ---------- */
  footer{
    border-top:1px solid var(--line);
    padding:42px 0;
  }
  .foot-row{
    display:flex; align-items:center; justify-content:space-between;
    flex-wrap:wrap; gap:20px;
  }
  .foot-row .brand{ font-size:17px; }
  .foot-links{ display:flex; gap:28px; font-size:13.5px; color:var(--ink-soft); }
  .foot-links a:hover{ color:var(--accent); }

  /* WhatsApp floating button */
  .float-wa{
    position:fixed; bottom:24px; right:24px; z-index:60;
    width:58px; height:58px; border-radius:50%;
    background:var(--accent);
    display:flex; align-items:center; justify-content:center;
    box-shadow:0 14px 30px -10px rgba(63,92,76,0.6);
    font-size:26px; color:#fff;
    animation:pulse 2.6s ease-in-out infinite;
  }
  @keyframes pulse{
    0%,100%{ box-shadow:0 14px 30px -10px rgba(63,92,76,0.6); }
    50%{ box-shadow:0 14px 30px -6px rgba(63,92,76,0.85), 0 0 0 8px rgba(63,92,76,0.12); }
  }

  /* Reveal on scroll */
  .reveal{ opacity:0; transform:translateY(24px); transition:opacity .7s ease, transform .7s ease; }
  .reveal.in{ opacity:1; transform:translateY(0); }

  /* ---------- Responsive ---------- */
  @media (max-width: 940px){
    .nav-links{ display:none; }
    .hero-grid, .about-grid, .loc-grid{ grid-template-columns:1fr; }
    .hero-visual{ height:380px; order:-1; }
    .service-grid{ grid-template-columns:1fr 1fr; }
    .process-row{ grid-template-columns:1fr; gap:44px; }
    .process-row::before{ display:none; }
    .proof .wrap{ gap:30px; }
  }
  @media (max-width: 560px){
    .wrap{ padding:0 20px; }
    .service-grid{ grid-template-columns:1fr; }
    .hero{ padding-top:48px; }
    .card-float{ padding:14px 16px; }
    .card-float.since{ display:none; }
  }
</style>
</head>
<body>

<header>
  <div class="nav">
    <div class="brand"><span class="brand-dot"></span>Dra. Lohrane Sousa</div>
    <nav class="nav-links">
      <a href="#servicos">Tratamentos</a>
      <a href="#sobre">Sobre</a>
      <a href="#localizacao">Localização</a>
    </nav>
    <a class="btn" href="https://tinyurl.com/agendamentodralohranesousa" target="_blank" rel="noopener">Agendar no WhatsApp</a>
  </div>
</header>

<main>
  <!-- HERO -->
  <section class="hero">
    <div class="wrap hero-grid">
      <div>
        <div class="eyebrow">Harmonização Facial &amp; Corporal · Centro, Curitiba</div>
        <h1>Cuidado que se percebe <em>antes</em> do resultado.</h1>
        <p class="hero-sub">Protocolos de estética facial e corporal pensados para a sua pele, no Edifício Santa Catarina, a poucos passos da Praça Santos Andrade.</p>
        <div class="hero-ctas">
          <a class="btn" href="https://tinyurl.com/agendamentodralohranesousa" target="_blank" rel="noopener">Agendar minha avaliação</a>
          <a class="btn btn-ghost" href="#localizacao">Ver endereço e horários</a>
        </div>
        <div class="rating-inline">
          <span class="stars">★★★★★</span>
          <span class="num">5,0</span>
          <span class="cap">— 23 avaliações no Google</span>
        </div>
      </div>
      <div class="hero-visual">
        <div class="blob blob-1"></div>
        <div class="blob blob-2"></div>
        <div class="card-float rating">
          <div class="icon-circle">★</div>
          <div>
            <div class="t1">5,0 de avaliação</div>
            <div class="t2">23 avaliações no Google</div>
          </div>
        </div>
        <div class="card-float since">
          <div class="icon-circle">📍</div>
          <div>
            <div class="t1">Centro de Curitiba</div>
            <div class="t2">Ed. Santa Catarina</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PROOF STRIP -->
  <section class="proof">
    <div class="wrap">
      <div class="proof-item"><strong>5,0★</strong> avaliação no Google</div>
      <div class="proof-divider"></div>
      <div class="proof-item"><strong>23</strong> avaliações verificadas</div>
      <div class="proof-divider"></div>
      <div class="proof-item"><strong>100%</strong> atendimento personalizado</div>
    </div>
  </section>

  <!-- SERVICES -->
  <section class="services" id="servicos">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">O que tratamos</div>
        <h2>Um protocolo para cada objetivo</h2>
        <p>Da limpeza de pele à harmonização corporal, cada procedimento é ajustado à sua rotina e ao resultado que você busca.</p>
      </div>
      <div class="service-grid">
        <div class="service-card reveal">
          <div class="service-petal">✦</div>
          <h3>Limpeza de pele</h3>
          <p>Higienização profunda que renova a textura e prepara a pele para os próximos cuidados.</p>
        </div>
        <div class="service-card reveal">
          <div class="service-petal">◍</div>
          <h3>Botox</h3>
          <p>Suavização de linhas de expressão com aplicação precisa e resultado natural.</p>
        </div>
        <div class="service-card reveal">
          <div class="service-petal">〜</div>
          <h3>Tratamentos corporais</h3>
          <p>Protocolos para contorno e firmeza, montados de acordo com o seu objetivo.</p>
        </div>
        <div class="service-card reveal">
          <div class="service-petal">◐</div>
          <h3>Enzimas locais e sistêmicas</h3>
          <p>Aplicações direcionadas para apoiar o metabolismo local da região tratada.</p>
        </div>
        <div class="service-card reveal">
          <div class="service-petal">✧</div>
          <h3>Microagulhamento</h3>
          <p>Estímulo de colágeno para uma pele com aspecto mais uniforme e renovado.</p>
        </div>
        <div class="service-card reveal">
          <div class="service-petal">◯</div>
          <h3>Skinbooster</h3>
          <p>Hidratação profunda que devolve viço e luminosidade à pele do rosto.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PROCESS -->
  <section class="process">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Como funciona</div>
        <h2>Do primeiro contato ao resultado</h2>
      </div>
      <div class="process-row">
        <div class="process-step reveal">
          <div class="process-num">1</div>
          <h3>Avaliação personalizada</h3>
          <p>Conversamos sobre sua pele, seu corpo e o que você espera do tratamento.</p>
        </div>
        <div class="process-step reveal">
          <div class="process-num">2</div>
          <h3>Plano sob medida</h3>
          <p>Você recebe um protocolo desenhado para o seu objetivo, sem procedimentos padronizados.</p>
        </div>
        <div class="process-step reveal">
          <div class="process-num">3</div>
          <h3>Acompanhamento contínuo</h3>
          <p>Ajustamos o plano ao longo do caminho, com atenção em cada retorno.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section class="about" id="sobre">
    <div class="wrap about-grid">
      <div class="about-visual reveal">
        <div class="about-blob">
          <span>"Cada paciente<br>merece um plano<br>só seu."</span>
        </div>
      </div>
      <div class="reveal">
        <div class="eyebrow">Quem cuida de você</div>
        <h2>Dra. Lohrane Sousa</h2>
        <p class="hero-sub" style="margin-top:20px; max-width:560px;">Especialista em harmonização facial e corporal, atende no Centro de Curitiba com um olhar atento para cada detalhe — do primeiro papo até o resultado final. O consultório fica no Edifício Santa Catarina, na Rua XV de Novembro.</p>
        <div class="quotes">
          <div class="quote">"Profissional boa e responsável, super recomendo para qualquer pessoa."<span>Avaliação no Google</span></div>
          <div class="quote">"Faz o possível para que cada paciente se sinta acolhido e cuidado."<span>Avaliação no Google</span></div>
          <div class="quote">"Uma dedicação que muda a experiência desde o primeiro contato."<span>Avaliação no Google</span></div>
        </div>
      </div>
    </div>
  </section>

  <!-- LOCATION -->
  <section class="location" id="localizacao">
    <div class="wrap loc-grid">
      <div class="reveal">
        <div class="eyebrow">Onde estamos</div>
        <h2>No coração do Centro de Curitiba</h2>
        <div class="loc-list">
          <div class="loc-item">
            <div class="loc-icon">📍</div>
            <div>
              <div class="t1">Edifício Santa Catarina</div>
              <div class="t2">R. XV de Novembro, 1222 — Sl 101, Centro, Curitiba - PR, 80060-000</div>
            </div>
          </div>
          <div class="loc-item">
            <div class="loc-icon">🕒</div>
            <div>
              <div class="t1">Horário de funcionamento</div>
              <div class="t2">Aberto hoje · fecha às 19h</div>
            </div>
          </div>
          <div class="loc-item">
            <div class="loc-icon">📞</div>
            <div>
              <div class="t1">(41) 99587-9618</div>
              <div class="t2">Ligue ou envie uma mensagem no WhatsApp</div>
            </div>
          </div>
          <div class="loc-item">
            <div class="loc-icon">✦</div>
            <div>
              <div class="t1">@dra.lohranesousa</div>
              <div class="t2">Acompanhe bastidores e resultados no Instagram</div>
            </div>
          </div>
        </div>
      </div>
      <div class="loc-card reveal">
        <div class="status"><span class="status-dot"></span>Aberto agora · fecha às 19h</div>
        <h3>Agende sua avaliação</h3>
        <p>Resposta rápida pelo WhatsApp para marcar seu horário e tirar dúvidas sobre o tratamento ideal para você.</p>
        <a class="btn" href="https://tinyurl.com/agendamentodralohranesousa" target="_blank" rel="noopener">Agendar agora →</a>
      </div>
    </div>
  </section>

  <!-- FINAL CTA -->
  <section class="final-cta">
    <div class="wrap">
      <h2 class="reveal">Sua avaliação começa com uma mensagem.</h2>
      <p class="reveal">Fale agora com a equipe da Dra. Lohrane Sousa e agende no horário que funcionar para você.</p>
      <a class="btn reveal" href="https://tinyurl.com/agendamentodralohranesousa" target="_blank" rel="noopener">Agendar minha avaliação</a>
    </div>
  </section>
</main>

<footer>
  <div class="wrap foot-row">
    <div class="brand"><span class="brand-dot"></span>Dra. Lohrane Sousa</div>
    <div class="foot-links">
      <a href="https://instagram.com/dra.lohranesousa/" target="_blank" rel="noopener">Instagram</a>
      <a href="https://maps.app.goo.gl/NuTtj5RkZpsueZHs5" target="_blank" rel="noopener">Localização</a>
      <a href="tel:+5541995879618">(41) 99587-9618</a>
    </div>
  </div>
</footer>

<a class="float-wa" href="https://tinyurl.com/agendamentodralohranesousa" target="_blank" rel="noopener" aria-label="Agendar no WhatsApp">💬</a>

<script>
  const revealEls = document.querySelectorAll('.reveal');
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target); }
    });
  }, { threshold: 0.15 });
  revealEls.forEach(el=> io.observe(el));
</script>

</body>
</html>
