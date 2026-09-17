# prefeito-de-valenca-do-piaui
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Prefeito de Valença do Piauí</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,600;0,9..144,700;1,9..144,500&family=Work+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg: #EDE3CB;
  --bg-alt: #E1D2AE;
  --surface: #FBF6E9;
  --surface-2: #F3E9D2;
  --ink: #3A2A1C;
  --ink-soft: #6E5A45;
  --line: #C9B78F;
  --terra: #B5502B;
  --terra-dark: #8E3C1F;
  --green: #46612F;
  --green-dark: #354A23;
  --blue: #386E85;
  --gold: #C99530;
  --red: #9C3A2C;
  --red-bg: #F1DCCF;
  --shadow: 2px 2px 0 rgba(58,42,28,0.18);
}
:root[data-theme="dark"]{
  --bg: #221A12;
  --bg-alt: #2C2116;
  --surface: #2E241A;
  --surface-2: #382C1E;
  --ink: #F2E6D2;
  --ink-soft: #C9B79A;
  --line: #4C3E2B;
  --terra: #D97A4D;
  --terra-dark: #E2905F;
  --green: #83A464;
  --green-dark: #9CBE7D;
  --blue: #7FB6CD;
  --gold: #E0B354;
  --red: #DD7C64;
  --red-bg: #3F2A22;
  --shadow: 2px 2px 0 rgba(0,0,0,0.35);
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){
    --bg: #221A12;
    --bg-alt: #2C2116;
    --surface: #2E241A;
    --surface-2: #382C1E;
    --ink: #F2E6D2;
    --ink-soft: #C9B79A;
    --line: #4C3E2B;
    --terra: #D97A4D;
    --terra-dark: #E2905F;
    --green: #83A464;
    --green-dark: #9CBE7D;
    --blue: #7FB6CD;
    --gold: #E0B354;
    --red: #DD7C64;
    --red-bg: #3F2A22;
    --shadow: 2px 2px 0 rgba(0,0,0,0.35);
  }
}

*{box-sizing:border-box;}
html,body{margin:0;padding:0;}
body{
  background: var(--bg);
  background-image:
    radial-gradient(circle at 15% 10%, var(--bg-alt) 0%, transparent 45%),
    radial-gradient(circle at 90% 85%, var(--bg-alt) 0%, transparent 40%);
  color: var(--ink);
  font-family: 'Work Sans', system-ui, -apple-system, sans-serif;
  min-height: 100vh;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
h1,h2,h3,.serif{
  font-family: 'Fraunces', Georgia, serif;
  font-weight: 600;
  letter-spacing: -0.01em;
  margin: 0;
}
.wrap{
  max-width: 760px;
  margin: 0 auto;
  padding: 28px 18px 60px;
}
a{color:inherit;}
button{font-family:inherit;}
::selection{background: var(--gold); color: var(--ink);}

/* ---------- Buttons ---------- */
.btn{
  display:inline-flex;
  align-items:center;
  gap:8px;
  justify-content:center;
  border: 2px solid var(--ink);
  background: var(--terra);
  color: #FBF6E9;
  font-family:'Work Sans', sans-serif;
  font-weight:600;
  font-size: 1rem;
  padding: 13px 22px;
  border-radius: 3px 14px 3px 14px;
  cursor: pointer;
  box-shadow: var(--shadow);
  transition: transform .12s ease, box-shadow .12s ease;
}
.btn:hover{ transform: translate(-2px,-2px); box-shadow: 4px 4px 0 rgba(58,42,28,0.22); }
.btn:active{ transform: translate(0,0); box-shadow: 1px 1px 0 rgba(58,42,28,0.22); }
.btn:focus-visible{ outline: 3px solid var(--blue); outline-offset: 2px; }
.btn.secondary{
  background: transparent;
  color: var(--ink);
  border-color: var(--line);
  box-shadow:none;
}
.btn.secondary:hover{ border-color: var(--ink); transform:none; box-shadow:none;}
.btn.full{width:100%;}
.btn:disabled{opacity:.45; cursor:not-allowed; transform:none; box-shadow:var(--shadow);}

/* ---------- Screens ---------- */
.screen{display:none;}
.screen.active{display:block; animation: fadeIn .35s ease;}
@keyframes fadeIn{ from{opacity:0; transform:translateY(6px);} to{opacity:1; transform:translateY(0);} }
@media (prefers-reduced-motion: reduce){
  .screen.active{animation:none;}
  .btn{transition:none;}
}

/* ---------- Intro ---------- */
.badge{
  display:inline-block;
  font-size:.78rem;
  color: var(--ink-soft);
  border:1px solid var(--line);
  padding: 3px 10px;
  border-radius: 20px;
  margin-bottom: 14px;
}
.hero-title{
  font-size: clamp(2.1rem, 7vw, 3.1rem);
  line-height: 1.05;
  color: var(--terra-dark);
}
.hero-sub{
  font-size: 1.1rem;
  color: var(--ink-soft);
  max-width: 46ch;
  margin-top: 12px;
}
.divider{
  height: 1px;
  background: repeating-linear-gradient(90deg, var(--line) 0 8px, transparent 8px 14px);
  margin: 26px 0;
}
.lore{
  background: var(--surface);
  border: 1px solid var(--line);
  border-radius: 4px 4px 4px 22px;
  padding: 20px 22px;
  margin: 18px 0;
}
.lore p{margin: 0 0 10px;}
.lore p:last-child{margin-bottom:0;}
.lore strong{color:var(--terra-dark);}

/* ---------- Character creation ---------- */
.field{margin-bottom: 22px;}
.field label{
  display:block;
  font-weight:600;
  margin-bottom: 8px;
}
.field input[type=text]{
  width:100%;
  padding: 12px 14px;
  border: 2px solid var(--line);
  border-radius: 4px;
  background: var(--surface);
  color: var(--ink);
  font-size: 1rem;
  font-family: inherit;
}
.field input[type=text]:focus-visible{outline: 3px solid var(--blue); outline-offset:1px; border-color: var(--blue);}
.field .hint{font-size:.85rem; color:var(--ink-soft); margin-top:6px;}

.option-grid{
  display:grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
}
@media (max-width: 560px){ .option-grid{grid-template-columns: 1fr;} }
.opt-card{
  text-align:left;
  border: 2px solid var(--line);
  background: var(--surface);
  border-radius: 4px 16px 4px 16px;
  padding: 15px 16px;
  cursor:pointer;
  transition: border-color .12s ease, transform .12s ease;
}
.opt-card:hover{ border-color: var(--terra); transform: translateY(-2px); }
.opt-card.selected{
  border-color: var(--terra);
  background: var(--surface-2);
  box-shadow: inset 0 0 0 1px var(--terra);
}
.opt-card h3{font-size:1.05rem; color: var(--terra-dark); margin-bottom:5px;}
.opt-card p{margin:0 0 8px; font-size:.92rem; color:var(--ink-soft);}
.opt-card .tags{font-size:.78rem; color: var(--green-dark); font-weight:600;}

/* ---------- Game HUD ---------- */
.hud{
  position: sticky;
  top: 0;
  z-index: 5;
  background: var(--bg);
  padding-top: 10px;
  padding-bottom: 12px;
  margin-bottom: 4px;
  border-bottom: 1px solid var(--line);
}
.hud-top{
  display:flex;
  justify-content:space-between;
  align-items:baseline;
  gap:10px;
  flex-wrap:wrap;
}
.hud-title{font-size: 1.15rem;}
.hud-turn{font-size:.85rem; color:var(--ink-soft);}
.progress{
  height:6px;
  background: var(--line);
  border-radius: 4px;
  margin: 10px 0 12px;
  overflow:hidden;
}
.progress-bar{height:100%; background: var(--terra); transition: width .3s ease;}
.stat-grid{
  display:grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 8px;
}
@media (max-width:520px){ .stat-grid{grid-template-columns: repeat(2,1fr);} }
.stat{
  background: var(--surface);
  border:1px solid var(--line);
  border-radius: 4px;
  padding: 7px 9px;
}
.stat .stat-label{font-size:.68rem; color:var(--ink-soft); display:flex; justify-content:space-between;}
.stat .stat-val{font-size:.95rem; font-weight:700;}
.stat .stat-bar{height:4px; background:var(--line); border-radius:3px; margin-top:4px; overflow:hidden;}
.stat .stat-bar i{display:block; height:100%; background: var(--green);}
.stat.caixa .stat-val{color: var(--terra-dark);}
.stat.low .stat-bar i{background: var(--red);}
.stat.mid .stat-bar i{background: var(--gold);}

/* ---------- Event / project cards ---------- */
.card{
  background: var(--surface);
  border: 1px solid var(--line);
  border-radius: 4px 22px 4px 4px;
  padding: 22px;
  margin-top: 18px;
}
.card-kicker{
  font-size:.78rem;
  font-weight:600;
  color: var(--green-dark);
  margin-bottom:6px;
}
.card-kicker.project{color:var(--blue);}
.card h2{font-size:1.35rem; color:var(--terra-dark); margin-bottom:10px;}
.card .body-text{color:var(--ink); margin-bottom:18px;}
.choice{
  display:block;
  width:100%;
  text-align:left;
  background: var(--surface-2);
  border: 2px solid var(--line);
  border-radius: 4px;
  padding: 13px 15px;
  margin-bottom: 10px;
  cursor:pointer;
  font-family: inherit;
  color: var(--ink);
  font-size: .96rem;
}
.choice:hover{border-color: var(--terra);}
.choice:focus-visible{outline:3px solid var(--blue); outline-offset:1px;}
.choice .choice-cost{display:block; font-size:.78rem; color:var(--ink-soft); margin-top:4px;}

.result-box{
  background: var(--surface-2);
  border-left: 4px solid var(--terra);
  border-radius: 2px 10px 10px 2px;
  padding: 16px 18px;
  margin-top: 16px;
}
.result-box p{margin:0 0 10px;}
.result-effects{
  display:flex;
  flex-wrap:wrap;
  gap:6px;
  margin: 6px 0 14px;
}
.eff{
  font-size:.78rem;
  font-weight:600;
  padding: 3px 9px;
  border-radius: 20px;
  background: var(--surface);
  border: 1px solid var(--line);
}
.eff.up{color: var(--green-dark);}
.eff.down{color: var(--red);}

/* ---------- End screen ---------- */
.end-banner{
  padding: 26px 22px;
  border-radius: 4px 26px 4px 26px;
  border: 1px solid var(--line);
  margin-bottom: 18px;
}
.end-banner.win{background: var(--surface-2); border-color: var(--green);}
.end-banner.lose{background: var(--red-bg); border-color: var(--red);}
.end-banner h2{font-size:1.6rem; margin-bottom:8px;}
.final-stats{
  display:grid;
  grid-template-columns: repeat(2,1fr);
  gap:10px;
  margin: 18px 0;
}
@media (max-width:480px){.final-stats{grid-template-columns:1fr;}}

.footer-note{
  text-align:center;
  font-size:.8rem;
  color:var(--ink-soft);
  margin-top: 34px;
}
.sr-only{position:absolute; width:1px; height:1px; overflow:hidden; clip:rect(0 0 0 0);}
</style>
</head>
<body>
<div class="wrap">

  <!-- ===================== INTRO ===================== -->
  <section id="screen-intro" class="screen active">
    <span class="badge">Simulador político &middot; 4 anos de mandato</span>
    <h1 class="hero-title">Prefeito de<br>Valença do Piauí</h1>
    <p class="hero-sub">O sertão espera. Cajueiros, buritizais e um povo que resiste à seca todo ano — e agora, à sua gestão. Assuma a prefeitura e decida, trimestre a trimestre, o destino da cidade.</p>

    <div class="divider"></div>

    <div class="lore">
      <p><strong>Valença do Piauí</strong> é uma cidade fictícia inspirada no sertão piauiense real: economia baseada na agricultura de sequeiro e na pecuária, cercada por caatinga e buritizais, com festas juninas movimentando o comércio e um clima semiárido que castiga o calendário de chuvas.</p>
      <p>Cerca de 14 mil habitantes vivem entre a sede e as zonas rurais. A cidade tem escolas lotadas, um posto de saúde que atende mais do que deveria, estradas de terra que viram lama em fevereiro e um açude que todo mundo observa com ansiedade em outubro.</p>
      <p>Você tem <strong>quatro anos</strong> — dezesseis trimestres — para equilibrar o orçamento, responder às crises e provar que sabe governar. No fim, o povo vota.</p>
    </div>

    <button class="btn full" id="btn-start" onclick="goToCharacterScreen()">Assumir a prefeitura</button>
  </section>

  <!-- ===================== CHARACTER CREATION ===================== -->
  <section id="screen-character" class="screen">
    <span class="badge">Antes de tomar posse</span>
    <h2 class="serif" style="font-size:1.8rem; margin-bottom:6px;">Quem é você?</h2>
    <p class="hero-sub" style="margin-bottom:20px;">Sua história define com o que você começa — e o que o povo espera de você.</p>

    <div class="field">
      <label for="input-name">Nome do(a) prefeito(a)</label>
      <input type="text" id="input-name" maxlength="28" placeholder="Ex.: Marlene Sá, Chico Brandão...">
    </div>

    <div class="field">
      <label for="input-slogan">Slogan de campanha</label>
      <input type="text" id="input-slogan" maxlength="46" placeholder="Ex.: Valença pra frente, sem deixar ninguém pra trás">
      <div class="hint">Vai aparecer no topo da sua gestão. Pode deixar em branco se preferir.</div>
    </div>

    <div class="field">
      <label>De onde você vem?</label>
      <div class="option-grid" id="bg-options"></div>
    </div>

    <button class="btn full" id="btn-inaugurate" onclick="beginGame()" disabled>Tomar posse</button>
  </section>

  <!-- ===================== GAME ===================== -->
  <section id="screen-game" class="screen">
    <div class="hud">
      <div class="hud-top">
        <div>
          <div class="hud-title serif" id="hud-mayor-name">—</div>
          <div class="hud-turn" id="hud-slogan"></div>
        </div>
        <div class="hud-turn" id="hud-turn-label">Ano 1 · 1º trimestre</div>
      </div>
      <div class="progress"><div class="progress-bar" id="progress-bar" style="width:0%"></div></div>
      <div class="stat-grid" id="stat-grid"></div>
    </div>

    <div id="game-stage"></div>
  </section>

  <!-- ===================== END ===================== -->
  <section id="screen-end" class="screen">
    <div id="end-content"></div>
    <button class="btn full" onclick="restartGame()">Começar novo mandato</button>
    <p class="footer-note">Valença do Piauí é uma cidade fictícia; os desafios se inspiram em questões reais do semiárido nordestino.</p>
  </section>

  <p class="footer-note" id="global-footer">Laboratório Arcade Social &middot; Simulador de Gestão Municipal</p>
</div>

<script>
/* =======================================================================
   ESTADO DO JOGO
   ======================================================================= */
const TOTAL_TURNS = 16; // 4 anos, 4 trimestres cada
const TRIMESTRES = ["1º trimestre","2º trimestre","3º trimestre","4º trimestre"];

const state = {
  name: "",
  slogan: "",
  background: null,
  turn: 0, // 0-indexed, 0..15
  stats: { educacao:50, saude:50, infra:45, ambiente:55, seguranca:50, popularidade:60 },
  caixa: 850,
  debtStreak: 0,
  lowPopStreak: 0,
  eventPool: [],
  projectPool: [],
  usedEvents: [],
  usedProjects: [],
  history: [],
  gameOver: false
};

/* =======================================================================
   DADOS: PERFIS INICIAIS
   ======================================================================= */
const BACKGROUNDS = [
  {
    id: "professora",
    title: "Professora(o) da rede pública",
    desc: "Trinta anos de sala de aula rural. Conhece cada família da zona rural pelo nome.",
    tags: "+Educação  +Popularidade  −Caixa",
    apply: s => { s.stats.educacao+=15; s.stats.popularidade+=5; s.caixa-=60; }
  },
  {
    id: "empresaria",
    title: "Empresário(a) do agronegócio",
    desc: "Dono(a) de uma casa de beneficiamento de caju. Sabe negociar, mas gera desconfiança.",
    tags: "+Caixa  +Infraestrutura  −Meio Ambiente  −Popularidade",
    apply: s => { s.caixa+=220; s.stats.infra+=8; s.stats.ambiente-=10; s.stats.popularidade-=5; }
  },
  {
    id: "engenheira",
    title: "Engenheiro(a) civil",
    desc: "Construiu metade das casas populares da cidade. Pensa em obra antes de discurso.",
    tags: "+Infraestrutura  +Segurança  −Caixa",
    apply: s => { s.stats.infra+=16; s.stats.seguranca+=4; s.caixa-=30; }
  },
  {
    id: "lideranca",
    title: "Liderança comunitária e sindical",
    desc: "Cresceu organizando feira e associação de moradores. O povo confia, o mercado nem tanto.",
    tags: "+Popularidade  +Saúde  −Caixa",
    apply: s => { s.stats.popularidade+=16; s.stats.saude+=6; s.caixa-=90; }
  }
];

/* =======================================================================
   DADOS: EVENTOS (crises e demandas do trimestre)
   ======================================================================= */
const EVENTS = [
[
  "Lixão a céu aberto na Vila Buriti",
  "Moradores da Vila Buriti denunciam um lixão irregular crescendo às margens do riacho, atraindo urubus e contaminando a água usada para lavar roupa.",
  [
    { label:"Construir um aterro controlado e coleta seletiva", cost:140, eff:{ambiente:14,saude:6,popularidade:6}, txt:"O aterro reduz a contaminação e a cidade ganha os primeiros pontos de coleta seletiva. As famílias vizinhas comemoram." },
    { label:"Fazer mutirão de limpeza e multar quem descartar irregularmente", cost:35, eff:{ambiente:6,popularidade:2,seguranca:2}, txt:"O mutirão limpa o local, mas sem aterro adequado o problema deve voltar em alguns meses." },
    { label:"Adiar — não há verba disponível agora", cost:0, eff:{ambiente:-8,popularidade:-6,saude:-3}, txt:"O lixão continua crescendo. Um vídeo do local circula nas redes e vira pauta de rádio local." }
  ]
],
[
  "Surto de dengue no bairro Sol Nascente",
  "Depois das primeiras chuvas, o posto de saúde registra um salto de casos de dengue. Os agentes de endemias pedem reforço urgente.",
  [
    { label:"Contratar agentes temporários e campanha porta a porta", cost:90, eff:{saude:14,popularidade:5}, txt:"Os agentes visitam quase todas as casas. Os casos começam a cair em três semanas." },
    { label:"Distribuir repelente e fazer campanha de rádio", cost:25, eff:{saude:5,popularidade:2}, txt:"A ação ajuda, mas sem visitas domiciliares alguns focos de mosquito continuam." },
    { label:"Aguardar orientação do estado", cost:0, eff:{saude:-12,popularidade:-8}, txt:"Os casos aumentam e o posto de saúde fica sobrecarregado. A imprensa regional cobra explicações." }
  ]
],
[
  "Pedido de acessibilidade na Praça da Matriz",
  "Um grupo de moradores com deficiência entrega um abaixo-assinado pedindo rampas, piso tátil e bancos adequados na praça central da cidade.",
  [
    { label:"Reformar a praça com acessibilidade completa", cost:110, eff:{infra:8,popularidade:8,saude:2}, txt:"A praça reformada vira modelo de acessibilidade na região. As famílias participam da inauguração." },
    { label:"Instalar apenas rampas nos pontos mais usados", cost:40, eff:{infra:4,popularidade:3}, txt:"Uma melhora parcial, mas o grupo pede que o restante da reforma continue no próximo trimestre." },
    { label:"Explicar que não há verba este trimestre", cost:0, eff:{popularidade:-6}, txt:"O grupo se sente ignorado e passa a acompanhar de perto as próximas decisões da prefeitura." }
  ]
],
[
  "Seca prolongada ameaça o açude municipal",
  "Já é setembro e não chove desde maio. O nível do açude que abastece parte da cidade está crítico.",
  [
    { label:"Perfurar poços artesianos e distribuir por carro-pipa", cost:160, eff:{saude:8,ambiente:2,popularidade:9,caixa_bonus:0}, txt:"A água chega às comunidades mais afetadas a tempo. Muita gente lembra dessa decisão na hora do voto." },
    { label:"Racionar o abastecimento e pedir economia à população", cost:20, eff:{popularidade:-3,saude:-2}, txt:"O racionamento evita o colapso total, mas gera filas e reclamações nos bairros mais distantes." },
    { label:"Aguardar as primeiras chuvas de outubro", cost:0, eff:{saude:-10,popularidade:-10,ambiente:-4}, txt:"Outubro demora a chegar. Famílias precisam buscar água em comunidades vizinhas." }
  ]
],
[
  "Erosão destrói estrada vicinal após temporal",
  "Uma chuva forte abriu uma vala de mais de um metro na estrada que liga a zona rural ao centro. Produtores não conseguem escoar a colheita.",
  [
    { label:"Reformar a estrada com drenagem adequada", cost:130, eff:{infra:12,popularidade:6}, txt:"A estrada fica pronta antes da próxima safra e os produtores voltam a escoar a produção normalmente." },
    { label:"Fazer um reparo emergencial com terraplenagem", cost:45, eff:{infra:4,popularidade:2}, txt:"O trânsito é liberado, mas a estrada deve sofrer o mesmo problema na próxima chuva forte." },
    { label:"Priorizar outras demandas este trimestre", cost:0, eff:{infra:-6,popularidade:-7}, txt:"Produtores relatam perdas na colheita por falta de escoamento. A associação rural cobra resposta." }
  ]
],
[
  "Falta de professores na escola rural do Riacho Fundo",
  "A escola municipal do Riacho Fundo está com duas turmas sem professor de matemática há mais de um mês.",
  [
    { label:"Abrir processo seletivo emergencial com bônus de deslocamento", cost:70, eff:{educacao:12,popularidade:4}, txt:"Duas professoras aceitam a vaga com o incentivo de transporte. As aulas voltam ao normal." },
    { label:"Remanejar um professor de outra escola por enquanto", cost:15, eff:{educacao:4}, txt:"A solução tampa o buraco, mas sobrecarrega a escola de origem." },
    { label:"Deixar para resolver no próximo semestre letivo", cost:0, eff:{educacao:-10,popularidade:-5}, txt:"Os alunos ficam meses sem aula da disciplina. Pais reclamam em reunião pública." }
  ]
],
[
  "Comerciantes pedem feira livre coberta",
  "A feira livre de sexta-feira, que reúne produtores de toda a região, ainda acontece ao relento — sol forte de manhã, poeira à tarde.",
  [
    { label:"Construir uma feira coberta com estrutura permanente", cost:150, eff:{infra:10,popularidade:8}, txt:"A feira coberta vira ponto de encontro e atrai feirantes de cidades vizinhas, aquecendo o comércio local." },
    { label:"Instalar toldos e melhorar os boxes existentes", cost:50, eff:{infra:4,popularidade:3}, txt:"Uma melhoria simples e bem recebida, mas sem grande impacto no movimento da feira." },
    { label:"Manter como está por ora", cost:0, eff:{popularidade:-3}, txt:"Os feirantes seguem reclamando informalmente, mas sem grande repercussão." }
  ]
],
[
  "Denúncia de desmatamento na mata do Riacho Fundo",
  "Fiscais flagram supressão irregular de vegetação nativa de caatinga para abertura de pasto, próximo a uma área de nascente.",
  [
    { label:"Embargar a área e reforçar fiscalização ambiental", cost:60, eff:{ambiente:14,popularidade:-2}, txt:"O embargo protege a nascente, mas o produtor autuado reclama publicamente da decisão." },
    { label:"Negociar um plano de recuperação com o proprietário", cost:30, eff:{ambiente:7,popularidade:3}, txt:"O acordo agrada as duas partes: a área começa a se recuperar e o produtor evita multa maior." },
    { label:"Não priorizar o caso agora", cost:0, eff:{ambiente:-10}, txt:"O desmatamento avança e a nascente começa a reduzir a vazão nos meses seguintes." }
  ]
],
[
  "Jovens pedem quadra poliesportiva no bairro periférico",
  "Um grupo de adolescentes do bairro Alto da Conquista pede um espaço de esporte e lazer, hoje inexistente na região.",
  [
    { label:"Construir quadra poliesportiva coberta", cost:120, eff:{seguranca:6,popularidade:9,saude:4}, txt:"A quadra vira point dos jovens à tarde e reduz relatos de pequenos conflitos no bairro." },
    { label:"Reformar um terreno baldio com trave e alambrado simples", cost:35, eff:{seguranca:3,popularidade:4}, txt:"Uma solução modesta, mas os jovens já começam a organizar campeonatos de fim de semana." },
    { label:"Explicar que não há terreno disponível", cost:0, eff:{popularidade:-4}, txt:"Os jovens seguem se reunindo em uma rua de terra, sem infraestrutura nenhuma." }
  ]
],
[
  "Idosos sem transporte para o posto de saúde",
  "Moradores da zona rural do Alto Bonito relatam que precisam andar mais de cinco quilômetros para chegar ao posto de saúde mais próximo.",
  [
    { label:"Criar linha de van rural com horário fixo", cost:75, eff:{saude:9,popularidade:6}, txt:"A van passa três vezes por semana e vira essencial para consultas e retirada de remédio." },
    { label:"Organizar caronas comunitárias com apoio de combustível", cost:20, eff:{saude:3,popularidade:2}, txt:"A solução ajuda em parte, mas depende da boa vontade de quem tem carro." },
    { label:"Sem recursos para isso agora", cost:0, eff:{saude:-6,popularidade:-5}, txt:"Idosos continuam faltando a consultas marcadas por falta de transporte." }
  ]
],
[
  "Artesãs de palha de buriti pedem apoio para o São João",
  "Um grupo de artesãs quer vender arranjos e utensílios de palha de buriti na festa junina, mas falta espaço de exposição e capital de giro.",
  [
    { label:"Montar uma feira de artesanato no São João com microcrédito", cost:65, eff:{popularidade:9,educacao:2}, txt:"As barracas vendem bem durante os três dias de festa e o grupo já planeja a próxima safra de palha." },
    { label:"Ceder apenas o espaço na praça, sem crédito", cost:15, eff:{popularidade:4}, txt:"As artesãs conseguem expor, mas reclamam da falta de capital para comprar mais matéria-prima." },
    { label:"Sugerir que procurem apoio no ano seguinte", cost:0, eff:{popularidade:-3}, txt:"O grupo vende por conta própria, na base da improvisação, como sempre fez." }
  ]
],
[
  "Falta de iluminação pública gera insegurança",
  "Moradores da Rua das Mangueiras relatam assaltos após o pôr do sol, num trecho sem nenhum poste funcionando há meses.",
  [
    { label:"Trocar toda a iluminação por LED e reforçar rondas", cost:95, eff:{seguranca:12,popularidade:5}, txt:"A rua volta a ter movimento à noite e os relatos de assalto praticamente somem." },
    { label:"Consertar apenas os postes mais críticos", cost:30, eff:{seguranca:5,popularidade:2}, txt:"A situação melhora, mas alguns trechos continuam escuros." },
    { label:"Registrar o pedido para análise futura", cost:0, eff:{seguranca:-8,popularidade:-6}, txt:"Um novo assalto é registrado na rua. Moradores organizam abaixo-assinado." }
  ]
],
[
  "Poço artesiano quebrado deixa comunidade sem água",
  "A bomba do único poço artesiano da comunidade Lagoa Seca quebrou. Famílias já caminham quilômetros para buscar água em baldes.",
  [
    { label:"Trocar a bomba e instalar reservatório de reserva", cost:80, eff:{saude:10,popularidade:6}, txt:"A água volta a circular normalmente e a comunidade ganha um reservatório extra para emergências." },
    { label:"Fazer um conserto simples e provisório", cost:25, eff:{saude:4,popularidade:2}, txt:"O poço volta a funcionar, mas o risco de quebrar de novo continua alto." },
    { label:"Priorizar outro investimento este trimestre", cost:0, eff:{saude:-9,popularidade:-7}, txt:"As famílias seguem dependendo de carros-pipa esporádicos." }
  ]
],
[
  "Reclamação de esgoto a céu aberto",
  "No bairro Vila Nova, o esgoto corre a céu aberto por falta de rede coletora, atraindo insetos e mau cheiro constante.",
  [
    { label:"Instalar rede de esgoto e estação de tratamento simples", cost:170, eff:{saude:14,ambiente:8,popularidade:7}, txt:"O bairro passa a ter saneamento básico pela primeira vez em sua história. Os casos de doenças ligadas à água caem." },
    { label:"Construir fossas sépticas comunitárias", cost:60, eff:{saude:6,ambiente:3,popularidade:3}, txt:"Uma solução intermediária que reduz o problema sem resolvê-lo por completo." },
    { label:"Deixar para um projeto maior no futuro", cost:0, eff:{saude:-8,ambiente:-4,popularidade:-5}, txt:"O cheiro e os riscos à saúde continuam incomodando os moradores." }
  ]
],
[
  "Pedido de reforma do posto de saúde central",
  "O único posto de saúde 24h da cidade está com o telhado furado e apenas um consultório funcionando plenamente.",
  [
    { label:"Reformar completamente e ampliar para dois consultórios", cost:145, eff:{saude:15,popularidade:7}, txt:"O posto reformado reduz o tempo de espera pela metade e vira orgulho da gestão." },
    { label:"Fazer reparo emergencial no telhado", cost:35, eff:{saude:5,popularidade:2}, txt:"O problema mais urgente é resolvido, mas a estrutura continua apertada para a demanda." },
    { label:"Adiar a reforma", cost:0, eff:{saude:-10,popularidade:-6}, txt:"Em dias de chuva, parte do posto precisa fechar por causa das goteiras." }
  ]
],
[
  "Fiscalização de agrotóxico perto do rio Piauí",
  "Denúncia aponta pulverização aérea de agrotóxico próxima às margens do rio, atingindo hortas comunitárias vizinhas.",
  [
    { label:"Fiscalizar, multar e criar zona de proteção ao redor do rio", cost:55, eff:{ambiente:12,saude:4,popularidade:-1}, txt:"A zona de proteção reduz a contaminação, embora alguns produtores critiquem a nova regra." },
    { label:"Apenas notificar o produtor responsável", cost:15, eff:{ambiente:4}, txt:"A notificação é registrada, mas sem fiscalização efetiva o problema pode se repetir." },
    { label:"Não investigar por falta de estrutura", cost:0, eff:{ambiente:-9,saude:-3}, txt:"As hortas comunitárias apresentam plantas queimadas nas semanas seguintes." }
  ]
],
[
  "Mototaxistas pedem regulamentação e pontos oficiais",
  "Cerca de 40 mototaxistas informais pedem pontos fixos, coletes de identificação e regras claras de funcionamento.",
  [
    { label:"Criar lei municipal com pontos, cadastro e capacitação", cost:45, eff:{seguranca:6,popularidade:7}, txt:"A categoria se organiza, os passageiros ganham mais segurança e a prefeitura arrecada uma taxa simples." },
    { label:"Autorizar pontos informais sem regulamentação completa", cost:10, eff:{popularidade:3}, txt:"Resolve parte do problema, mas sem fiscalização o serviço segue desorganizado." },
    { label:"Deixar como está", cost:0, eff:{popularidade:-4}, txt:"Os mototaxistas seguem brigando por pontos informais nas esquinas mais movimentadas." }
  ]
],
[
  "Comunidade quilombola pede reconhecimento e infraestrutura",
  "A comunidade Baixão dos Ferreira, remanescente de quilombo, pede apoio para regularização fundiária, água encanada e uma escola mais próxima.",
  [
    { label:"Apoiar a regularização e levar água encanada à comunidade", cost:135, eff:{infra:7,saude:8,popularidade:9}, txt:"A comunidade recebe pela primeira vez água encanada regular, e o processo de regularização avança." },
    { label:"Levar apenas um caminhão-pipa periódico", cost:30, eff:{saude:3,popularidade:2}, txt:"Uma ajuda pontual que não resolve a questão de fundo, mas alivia o dia a dia." },
    { label:"Encaminhar o pedido ao governo estadual", cost:0, eff:{popularidade:-5}, txt:"O processo trava na burocracia estadual e a comunidade sente que a prefeitura se eximiu do problema." }
  ]
],
[
  "Enchente atinge o bairro Baixa do Rio",
  "Uma chuva forte de fevereiro faz o riacho transbordar e inunda dezenas de casas na parte baixa da cidade.",
  [
    { label:"Abrigar as famílias, limpar e iniciar obra de drenagem", cost:150, eff:{infra:10,saude:6,popularidade:8}, txt:"A drenagem reduz o risco de novas enchentes e as famílias voltam para casas mais seguras." },
    { label:"Prestar apoio emergencial sem obra estrutural", cost:50, eff:{saude:3,popularidade:3}, txt:"A situação imediata é atendida, mas o bairro continua vulnerável à próxima chuva forte." },
    { label:"Aguardar recursos estaduais para a obra", cost:0, eff:{infra:-5,popularidade:-8}, txt:"Sem resposta rápida, moradores organizam protesto em frente à prefeitura." }
  ]
],
[
  "Convite para consórcio regional de tratamento de lixo",
  "Cidades vizinhas convidam Valença do Piauí a entrar num consórcio para construir um aterro sanitário regional, dividindo custos.",
  [
    { label:"Entrar no consórcio e investir na cota municipal", cost:100, eff:{ambiente:10,infra:3,popularidade:2}, txt:"O consórcio reduz o custo por cidade e Valença passa a descartar o lixo de forma correta." },
    { label:"Aguardar mais uma reunião antes de decidir", cost:0, eff:{popularidade:-1}, txt:"A decisão é adiada. As outras cidades seguem sem Valença por enquanto." },
    { label:"Recusar o convite para não comprometer o orçamento", cost:0, eff:{ambiente:-5}, txt:"O município mantém o descarte como está, sem o suporte do consórcio regional." }
  ]
],
[
  "Horta escolar comunitária na Escola Municipal Dom Barreto",
  "Professoras propõem uma horta comunitária na escola, envolvendo alunos e famílias na produção de hortaliças para a merenda.",
  [
    { label:"Financiar a horta com apoio técnico da secretaria de agricultura", cost:35, eff:{educacao:6,saude:4,ambiente:3,popularidade:3}, txt:"A horta vira parte do currículo e melhora a merenda escolar com produtos frescos." },
    { label:"Ceder apenas as sementes e ferramentas básicas", cost:12, eff:{educacao:2,popularidade:1}, txt:"A horta começa pequena, sustentada principalmente pelo esforço voluntário das professoras." },
    { label:"Adiar o projeto para o próximo ano letivo", cost:0, eff:{educacao:-2}, txt:"A ideia fica engavetada e as professoras seguem cobrando uma resposta." }
  ]
],
[
  "Praga na lavoura de milho preocupa pequenos agricultores",
  "Uma lagarta está destruindo plantações de milho de agricultura familiar, ameaçando a safra de várias famílias da zona rural.",
  [
    { label:"Distribuir defensivo biológico e orientação técnica gratuita", cost:70, eff:{ambiente:5,popularidade:7}, txt:"O controle biológico contém a praga sem agredir o solo, e a safra é parcialmente salva." },
    { label:"Distribuir apenas informativo sobre o manejo da praga", cost:10, eff:{popularidade:2}, txt:"A orientação ajuda alguns produtores mais atentos, mas a maioria perde parte da colheita." },
    { label:"Não intervir — é uma questão estadual", cost:0, eff:{popularidade:-6}, txt:"Várias famílias perdem boa parte da safra de milho daquele ano." }
  ]
],
[
  "Rádio comunitária pede transparência nas contas",
  "A rádio local pede acesso aos gastos da prefeitura para um programa semanal de prestação de contas ao público.",
  [
    { label:"Criar portal da transparência e ceder entrevista mensal", cost:20, eff:{popularidade:8}, txt:"A iniciativa é bem recebida e passa a imagem de uma gestão aberta ao diálogo." },
    { label:"Enviar apenas os relatórios obrigatórios por lei", cost:5, eff:{popularidade:2}, txt:"O mínimo é cumprido, sem gerar grande repercussão." },
    { label:"Recusar a entrevista por enquanto", cost:0, eff:{popularidade:-7}, txt:"A rádio comenta a recusa no ar, o que gera desconfiança entre os ouvintes." }
  ]
]
];

/* =======================================================================
   DADOS: PROJETOS DE INVESTIMENTO
   ======================================================================= */
const PROJECTS = [
[
  "Pavimentação de ruas do centro",
  "A equipe de obras apresenta um plano para pavimentar as ruas mais movimentadas do centro comercial, hoje de terra batida.",
  [
    { label:"Pavimentação completa com drenagem", cost:180, eff:{infra:16,popularidade:6}, txt:"As ruas centrais ficam transitáveis mesmo em dias de chuva forte, valorizando os imóveis da região." },
    { label:"Pavimentação simples, sem drenagem", cost:90, eff:{infra:8,popularidade:3}, txt:"Uma melhora perceptível, mas os primeiros temporais já mostram poças em alguns pontos." },
    { label:"Guardar o recurso para outra prioridade", cost:0, eff:{infra:0}, txt:"O orçamento fica reservado. As ruas seguem como estavam." }
  ]
],
[
  "Reforma das escolas municipais",
  "Um levantamento aponta salas de aula com carteiras quebradas, ventiladores parados e banheiros precisando de reparo em três escolas.",
  [
    { label:"Reformar as três escolas por completo", cost:160, eff:{educacao:16,popularidade:6}, txt:"As escolas ganham salas mais confortáveis, e professores relatam mais engajamento dos alunos." },
    { label:"Reformar apenas a escola em pior estado", cost:70, eff:{educacao:7,popularidade:2}, txt:"A escola mais crítica melhora, mas as outras duas seguem precisando de reparo." },
    { label:"Adiar a reforma para o próximo ano", cost:0, eff:{educacao:-3}, txt:"Professores continuam improvisando aulas com a estrutura que têm." }
  ]
],
[
  "Sistema de coleta seletiva municipal",
  "A secretaria de meio ambiente propõe implantar coleta seletiva porta a porta, com uma cooperativa de catadores como parceira.",
  [
    { label:"Implantar coleta seletiva completa com a cooperativa", cost:110, eff:{ambiente:14,popularidade:5}, txt:"A cooperativa gera renda para dezenas de famílias e o volume de lixo em aterro cai significativamente." },
    { label:"Implantar apenas em bairros centrais", cost:45, eff:{ambiente:6,popularidade:2}, txt:"Um começo modesto, mas que já reduz parte do lixo descartado incorretamente." },
    { label:"Não investir neste trimestre", cost:0, eff:{ambiente:0}, txt:"A coleta seletiva continua sendo apenas um projeto no papel." }
  ]
],
[
  "Cisternas para captação de água de chuva",
  "Uma ONG parceira oferece cofinanciar cisternas de placa nas comunidades rurais mais afetadas pela seca.",
  [
    { label:"Construir cisternas em todas as comunidades prioritárias", cost:130, eff:{saude:10,ambiente:5,popularidade:7}, txt:"As famílias passam a ter reserva própria de água mesmo nos meses mais secos do ano." },
    { label:"Construir cisternas apenas na comunidade mais crítica", cost:55, eff:{saude:5,popularidade:3}, txt:"A comunidade mais afetada melhora, mas as demais seguem dependendo de carro-pipa." },
    { label:"Não aderir à parceria por ora", cost:0, eff:{saude:0}, txt:"A oferta da ONG expira e pode não se repetir tão cedo." }
  ]
],
[
  "Iluminação em LED para toda a cidade",
  "Um estudo mostra que trocar toda a iluminação pública por LED reduziria o gasto de energia e aumentaria a segurança noturna.",
  [
    { label:"Trocar toda a iluminação da cidade", cost:150, eff:{seguranca:14,infra:4,popularidade:5}, txt:"A cidade fica visivelmente mais segura à noite, e a conta de energia da prefeitura cai nos meses seguintes." },
    { label:"Trocar apenas nos bairros mais escuros", cost:60, eff:{seguranca:6,popularidade:2}, txt:"Os pontos mais críticos melhoram, mas parte da cidade segue mal iluminada." },
    { label:"Adiar o investimento", cost:0, eff:{seguranca:0}, txt:"A iluminação antiga continua consumindo mais energia e falhando com frequência." }
  ]
],
[
  "Parque municipal e área de lazer",
  "Um terreno público abandonado no centro poderia virar um parque com área verde, pista de caminhada e playground.",
  [
    { label:"Construir o parque completo com área verde e playground", cost:140, eff:{ambiente:8,saude:5,popularidade:9}, txt:"O parque vira point de fim de tarde da cidade, com famílias caminhando e crianças brincando." },
    { label:"Fazer apenas uma limpeza e cercamento do terreno", cost:35, eff:{ambiente:2,popularidade:2}, txt:"O terreno deixa de ser um depósito de lixo, mas ainda não vira um espaço de lazer de fato." },
    { label:"Vender o terreno para gerar receita", cost:0, eff:{caixa_bonus:80,popularidade:-4,ambiente:-3}, txt:"O caixa melhora no curto prazo, mas moradores lamentam a perda de um possível espaço verde." }
  ]
],
[
  "Ciclovia ligando os bairros ao centro",
  "Estudantes e trabalhadores que pedalam diariamente pedem uma ciclovia segura entre os bairros periféricos e o centro.",
  [
    { label:"Construir ciclovia completa com sinalização", cost:100, eff:{infra:8,seguranca:4,popularidade:6}, txt:"O número de ciclistas cresce e os acidentes na via principal caem." },
    { label:"Pintar apenas uma faixa compartilhada", cost:30, eff:{seguranca:2,popularidade:2}, txt:"Uma solução barata que ajuda pouco, já que os carros seguem invadindo a faixa." },
    { label:"Não investir neste trimestre", cost:0, eff:{seguranca:0}, txt:"Ciclistas continuam dividindo a pista com carros e caminhões." }
  ]
],
[
  "Festival Cultural de Valença: forró, cajuína e artesanato",
  "A secretaria de cultura propõe transformar a tradicional festa de fim de safra em um festival regional, atraindo turistas das cidades vizinhas.",
  [
    { label:"Investir em um festival de três dias com palco, feira e oficinas", cost:95, eff:{popularidade:12,educacao:2}, txt:"O festival lota a praça central, movimenta o comércio local e vira tradição na região." },
    { label:"Fazer uma festa simples de um dia", cost:35, eff:{popularidade:5}, txt:"A festa agrada, mas fica pequena perto do potencial da cidade." },
    { label:"Cancelar por causa do orçamento", cost:0, eff:{popularidade:-5}, txt:"Moradores lamentam a ausência da festa mais esperada do ano." }
  ]
],
[
  "Rede de saneamento básico ampliada",
  "Um diagnóstico da secretaria de saúde aponta que menos da metade da cidade tem rede de esgoto adequada.",
  [
    { label:"Ampliar a rede de esgoto para os bairros restantes", cost:190, eff:{saude:14,ambiente:8,popularidade:7}, txt:"A cobertura de saneamento quase dobra, reduzindo casos de doenças de veiculação hídrica." },
    { label:"Ampliar parcialmente, priorizando um bairro", cost:80, eff:{saude:6,ambiente:3,popularidade:3}, txt:"Um bairro melhora bastante, mas os demais seguem na fila de espera." },
    { label:"Adiar o investimento", cost:0, eff:{saude:0}, txt:"A cobertura de saneamento permanece baixa por mais um ano." }
  ]
],
[
  "Capacitação profissional para jovens",
  "O SENAI regional oferece parceria para cursos técnicos gratuitos, desde que a prefeitura garanta transporte e espaço.",
  [
    { label:"Firmar a parceria completa com bolsa-transporte", cost:60, eff:{educacao:10,popularidade:6}, txt:"Dezenas de jovens se formam em cursos técnicos e vários conseguem os primeiros empregos formais da cidade." },
    { label:"Oferecer apenas o espaço, sem bolsa-transporte", cost:15, eff:{educacao:4,popularidade:2}, txt:"Alguns jovens da zona rural desistem por não conseguir chegar até as aulas." },
    { label:"Não firmar a parceria este ano", cost:0, eff:{educacao:0}, txt:"A oportunidade de capacitação gratuita passa longe de Valença do Piauí." }
  ]
],
[
  "Reforço do corpo de guardas municipais",
  "O comando da guarda municipal pede mais efetivo e viaturas para cobrir zonas rurais que hoje ficam sem nenhuma ronda.",
  [
    { label:"Contratar mais guardas e comprar viaturas novas", cost:120, eff:{seguranca:13,popularidade:5}, txt:"As zonas rurais passam a ter ronda regular pela primeira vez, e a sensação de segurança melhora bastante." },
    { label:"Reforçar apenas o efetivo, sem viaturas novas", cost:45, eff:{seguranca:5,popularidade:2}, txt:"Mais guardas ajudam, mas a falta de viaturas limita o alcance das rondas." },
    { label:"Manter o efetivo atual", cost:0, eff:{seguranca:0}, txt:"As zonas rurais continuam praticamente sem presença da guarda municipal." }
  ]
],
[
  "Recuperação da mata ciliar do rio Piauí",
  "Técnicos ambientais propõem um projeto de reflorestamento nas margens do rio, hoje degradadas pelo pisoteio de gado e erosão.",
  [
    { label:"Reflorestar toda a margem com mudas nativas", cost:75, eff:{ambiente:15,popularidade:4}, txt:"As margens do rio começam a se recuperar, reduzindo o assoreamento e melhorando a qualidade da água." },
    { label:"Reflorestar apenas o trecho mais crítico", cost:30, eff:{ambiente:7,popularidade:2}, txt:"O trecho mais degradado começa a se recuperar, mas o restante da margem segue exposto." },
    { label:"Não investir neste trimestre", cost:0, eff:{ambiente:0}, txt:"A erosão nas margens do rio continua avançando aos poucos." }
  ]
]
];

/* =======================================================================
   HELPERS
   ======================================================================= */
function shuffle(arr){
  const a = arr.slice();
  for(let i=a.length-1;i>0;i--){
    const j = Math.floor(Math.random()*(i+1));
    [a[i],a[j]]=[a[j],a[i]];
  }
  return a;
}

function drawFrom(poolName){
  const usedKey = poolName === 'events' ? 'usedEvents' : 'usedProjects';
  const sourceArr = poolName === 'events' ? EVENTS : PROJECTS;
  if(state[poolName].length === 0){
    // reshuffle a fresh pool, avoiding immediate repeat of the very last used one when possible
    let fresh = shuffle(sourceArr.map((_,i)=>i));
    state[poolName] = fresh;
  }
  const idx = state[poolName].pop();
  state[usedKey].push(idx);
  return sourceArr[idx];
}

function clamp(v){ return Math.max(0, Math.min(100, v)); }

function fmtMoney(v){
  const sign = v < 0 ? "-" : "";
  return `${sign}R$ ${Math.abs(Math.round(v))} mil`;
}

function showScreen(id){
  document.querySelectorAll(".screen").forEach(s=>s.classList.remove("active"));
  document.getElementById(id).classList.add("active");
  window.scrollTo({top:0, behavior:"instant" in window ? "instant":"auto"});
}

/* =======================================================================
   TELA 1 -> 2: CRIAÇÃO DE PERSONAGEM
   ======================================================================= */
function goToCharacterScreen(){
  const grid = document.getElementById("bg-options");
  grid.innerHTML = "";
  BACKGROUNDS.forEach(bg=>{
    const div = document.createElement("div");
    div.className = "opt-card";
    div.setAttribute("role","button");
    div.setAttribute("tabindex","0");
    div.innerHTML = `<h3>${bg.title}</h3><p>${bg.desc}</p><div class="tags">${bg.tags}</div>`;
    div.onclick = () => selectBackground(bg.id, div);
    div.onkeydown = (e) => { if(e.key === "Enter" || e.key === " "){ e.preventDefault(); selectBackground(bg.id, div); } };
    grid.appendChild(div);
  });
  showScreen("screen-character");
}

function selectBackground(id, el){
  state.background = id;
  document.querySelectorAll(".opt-card").forEach(c=>c.classList.remove("selected"));
  el.classList.add("selected");
  document.getElementById("btn-inaugurate").disabled = false;
}

/* =======================================================================
   INÍCIO DO JOGO
   ======================================================================= */
function beginGame(){
  const nameInput = document.getElementById("input-name").value.trim();
  const sloganInput = document.getElementById("input-slogan").value.trim();
  state.name = nameInput || "Prefeito(a) de Valença";
  state.slogan = sloganInput;

  const bg = BACKGROUNDS.find(b=>b.id===state.background);
  if(bg) bg.apply(state);

  state.caixa = Math.round(state.caixa);
  Object.keys(state.stats).forEach(k=> state.stats[k] = clamp(state.stats[k]));

  document.getElementById("hud-mayor-name").textContent = state.name;
  document.getElementById("hud-slogan").textContent = state.slogan ? `“${state.slogan}”` : "Valença do Piauí";

  showScreen("screen-game");
  renderTurn();
}

/* =======================================================================
   HUD
   ======================================================================= */
const STAT_META = {
  educacao:{label:"Educação"},
  saude:{label:"Saúde"},
  infra:{label:"Infraestrutura"},
  ambiente:{label:"Meio ambiente"},
  seguranca:{label:"Segurança"},
  popularidade:{label:"Popularidade"}
};

function renderHUD(){
  const year = Math.floor(state.turn/4)+1;
  const q = TRIMESTRES[state.turn%4];
  document.getElementById("hud-turn-label").textContent = `Ano ${year} · ${q}`;
  document.getElementById("progress-bar").style.width = `${(state.turn/TOTAL_TURNS)*100}%`;

  const grid = document.getElementById("stat-grid");
  grid.innerHTML = "";

  const caixaDiv = document.createElement("div");
  caixaDiv.className = "stat caixa";
  caixaDiv.innerHTML = `<div class="stat-label"><span>Caixa</span></div><div class="stat-val">${fmtMoney(state.caixa)}</div>`;
  grid.appendChild(caixaDiv);

  Object.entries(STAT_META).forEach(([key,meta])=>{
    const val = clamp(state.stats[key]);
    const div = document.createElement("div");
    div.className = "stat" + (val < 35 ? " low" : val < 60 ? " mid":"");
    div.innerHTML = `<div class="stat-label"><span>${meta.label}</span><span>${val}</span></div>
      <div class="stat-bar"><i style="width:${val}%"></i></div>`;
    grid.appendChild(div);
  });
}

/* =======================================================================
   RODADA: EVENTO -> PROJETO -> AVANÇAR
   ======================================================================= */
function renderTurn(){
  if(state.gameOver) return;
  renderHUD();
  const ev = drawFrom('eventPool');
  renderCard(ev, "event", "Demanda do trimestre", () => renderProject());
}

function renderProject(){
  renderHUD();
  const pr = drawFrom('projectPool');
  renderCard(pr, "project", "Projeto de investimento", () => advanceTurn());
}

function renderCard(data, kind, kicker, onDone){
  const [title, text, options] = data;
  const stage = document.getElementById("game-stage");
  stage.innerHTML = "";

  const card = document.createElement("div");
  card.className = "card";
  card.innerHTML = `
    <div class="card-kicker ${kind==='project'?'project':''}">${kicker}</div>
    <h2>${title}</h2>
    <p class="body-text">${text}</p>
  `;

  const choicesWrap = document.createElement("div");
  options.forEach(opt=>{
    const btn = document.createElement("button");
    btn.className = "choice";
    const costLabel = opt.cost > 0 ? `Custo estimado: ${fmtMoney(opt.cost)}` : "Sem custo direto";
    btn.innerHTML = `${opt.label}<span class="choice-cost">${costLabel}</span>`;
    btn.onclick = () => resolveChoice(card, choicesWrap, opt, onDone);
    choicesWrap.appendChild(btn);
  });
  card.appendChild(choicesWrap);
  stage.appendChild(card);
}

function resolveChoice(card, choicesWrap, opt, onDone){
  // apply effects
  state.caixa -= (opt.cost||0);
  if(opt.eff.caixa_bonus) state.caixa += opt.eff.caixa_bonus;
  Object.keys(opt.eff).forEach(k=>{
    if(k==='caixa_bonus') return;
    state.stats[k] = clamp((state.stats[k]||0) + opt.eff[k]);
  });

  choicesWrap.remove();

  const box = document.createElement("div");
  box.className = "result-box";
  const effTags = Object.entries(opt.eff).map(([k,v])=>{
    if(k==='caixa_bonus'){
      return `<span class="eff ${v>=0?'up':'down'}">Caixa ${v>=0?'+':''}${v}</span>`;
    }
    const label = STAT_META[k] ? STAT_META[k].label : k;
    return `<span class="eff ${v>=0?'up':'down'}">${label} ${v>=0?'+':''}${v}</span>`;
  }).join("");
  box.innerHTML = `<p>${opt.txt}</p><div class="result-effects">${effTags}</div>`;

  const nextBtn = document.createElement("button");
  nextBtn.className = "btn full";
  nextBtn.textContent = "Continuar";
  nextBtn.onclick = onDone;
  box.appendChild(nextBtn);

  card.appendChild(box);
  renderHUD();
  checkEarlyGameOver();
}

/* =======================================================================
   CONDIÇÕES DE FIM ANTECIPADO
   ======================================================================= */
function checkEarlyGameOver(){
  if(state.caixa < -250){
    state.debtStreak++;
  } else {
    state.debtStreak = 0;
  }
  if(state.stats.popularidade <= 10){
    state.lowPopStreak++;
  } else {
    state.lowPopStreak = 0;
  }

  if(state.debtStreak >= 2){
    endGame("intervencao");
  } else if(state.lowPopStreak >= 2){
    endGame("impeachment");
  }
}

/* =======================================================================
   AVANÇAR TURNO
   ======================================================================= */
function advanceTurn(){
  if(state.gameOver) return;

  // receita trimestral simples com base na infraestrutura e educação
  const receita = 95 + Math.round(state.stats.infra*0.9) + Math.round(state.stats.educacao*0.35) - 55;
  state.caixa += receita;

  state.history.push({turn:state.turn, caixa:state.caixa, ...state.stats});
  state.turn++;

  if(state.turn >= TOTAL_TURNS){
    endGame("eleicao");
    return;
  }
  renderTurn();
}

/* =======================================================================
   FIM DE JOGO
   ======================================================================= */
function endGame(reason){
  state.gameOver = true;
  showScreen("screen-end");
  const content = document.getElementById("end-content");
  const s = state.stats;
  const avg = (s.educacao + s.saude + s.infra + s.ambiente + s.seguranca) / 5;

  let bannerClass, title, body;

  if(reason === "intervencao"){
    bannerClass = "lose";
    title = "Intervenção do Tribunal de Contas";
    body = `As contas de ${state.name} ficaram no vermelho por trimestres seguidos. O Tribunal de Contas do Estado interveio na gestão antes do fim do mandato. Valença do Piauí segue com uma junta interventora até novas eleições.`;
  } else if(reason === "impeachment"){
    bannerClass = "lose";
    title = "Processo de impeachment";
    body = `A popularidade de ${state.name} despencou e se manteve crítica por trimestres seguidos. A Câmara Municipal abriu processo de impeachment, encerrando o mandato antes da eleição seguinte.`;
  } else {
    const win = s.popularidade >= 50 && avg >= 45;
    bannerClass = win ? "win" : "lose";
    if(s.popularidade >= 70 && avg >= 65){
      title = "Reeleito(a) com ampla vantagem";
      body = `${state.name} termina o mandato com o reconhecimento nítido da população de Valença do Piauí. Nas urnas, a vitória vem tranquila, com discurso lembrando das obras e das crises enfrentadas juntos.`;
    } else if(win){
      title = "Reeleito(a) por uma margem apertada";
      body = `A votação é disputada, mas ${state.name} garante mais quatro anos à frente da prefeitura. A cidade avançou em algumas frentes, mas o eleitorado deixou claro que espera mais no próximo mandato.`;
    } else if(s.popularidade >= 35){
      title = "Derrota nas urnas";
      body = `Depois de quatro anos de decisões difíceis, ${state.name} não consegue convencer a maioria do eleitorado e perde a disputa pela reeleição. O adversário promete continuar parte dos projetos iniciados.`;
    } else {
      title = "Derrota expressiva";
      body = `O desgaste acumulado ao longo do mandato é grande demais. ${state.name} termina a disputa eleitoral em desvantagem clara, e a oposição já anuncia mudanças de rumo para a cidade.`;
    }
  }

  const finalStatsHTML = Object.entries(STAT_META).map(([k,meta])=>{
    const v = clamp(s[k]);
    return `<div class="stat${v<35?' low':v<60?' mid':''}">
      <div class="stat-label"><span>${meta.label}</span><span>${v}</span></div>
      <div class="stat-bar"><i style="width:${v}%"></i></div>
    </div>`;
  }).join("");

  content.innerHTML = `
    <span class="badge">Fim de mandato · Ano ${Math.min(4, Math.floor(state.turn/4)+ (state.turn%4===0?0:1))}</span>
    <div class="end-banner ${bannerClass}">
      <h2 class="serif">${title}</h2>
      <p>${body}</p>
    </div>
    <h3 class="serif" style="margin-bottom:10px;">Balanço final de Valença do Piauí</h3>
    <div class="final-stats">
      <div class="stat caixa"><div class="stat-label"><span>Caixa final</span></div><div class="stat-val">${fmtMoney(state.caixa)}</div></div>
      ${finalStatsHTML}
    </div>
  `;
}

/* =======================================================================
   REINICIAR
   ======================================================================= */
function restartGame(){
  state.name = ""; state.slogan = ""; state.background = null;
  state.turn = 0;
  state.stats = { educacao:50, saude:50, infra:45, ambiente:55, seguranca:50, popularidade:60 };
  state.caixa = 850;
  state.debtStreak = 0; state.lowPopStreak = 0;
  state.eventPool = []; state.projectPool = [];
  state.usedEvents = []; state.usedProjects = [];
  state.history = [];
  state.gameOver = false;
  document.getElementById("input-name").value = "";
  document.getElementById("input-slogan").value = "";
  document.getElementById("btn-inaugurate").disabled = true;
  showScreen("screen-intro");
}
</script>
</body>
</html>
