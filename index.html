<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>PrismaLab | Simulador de prismas</title>
  <style>
    /* ---------- Sistema visual ---------- */
    :root {
      --ink: #17213b;
      --muted: #66708f;
      --paper: #f7f9ff;
      --card: #ffffff;
      --line: #e4e9f5;
      --primary: #6557f5;
      --primary-dark: #4c41c9;
      --teal: #10b9b0;
      --orange: #ff9f43;
      --pink: #ee6092;
      --green: #22b573;
      --danger: #e45667;
      --shadow: 0 16px 44px rgba(47, 55, 105, .12);
      --radius: 22px;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      color: var(--ink);
      background:
        radial-gradient(circle at 4% 0%, rgba(101,87,245,.12), transparent 27rem),
        radial-gradient(circle at 100% 20%, rgba(16,185,176,.10), transparent 24rem),
        var(--paper);
      font: 16px/1.5 Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
    button, input, select { font: inherit; }
    button { cursor: pointer; }
    :focus-visible { outline: 3px solid rgba(101, 87, 245, .35); outline-offset: 3px; }

    .app-shell { max-width: 1250px; margin: 0 auto; padding: 22px 22px 52px; }
    .topbar {
      display: flex; align-items: center; justify-content: space-between; gap: 18px;
      margin-bottom: 24px;
    }
    .brand { display: flex; align-items: center; gap: 12px; font-weight: 900; letter-spacing: -.03em; }
    .brand-mark {
      width: 42px; height: 42px; display: grid; place-items: center; border-radius: 14px;
      color: white; background: linear-gradient(135deg, var(--primary), var(--pink));
      box-shadow: 0 8px 20px rgba(101,87,245,.25); font-size: 22px;
    }
    .brand small { display: block; color: var(--muted); font-size: 11px; letter-spacing: .06em; text-transform: uppercase; }
    .top-actions { display: flex; align-items: center; gap: 10px; }

    .btn {
      border: 0; border-radius: 13px; padding: 11px 16px; font-weight: 800;
      transition: transform .18s ease, box-shadow .18s ease, background .18s ease;
    }
    .btn:hover { transform: translateY(-2px); }
    .btn-primary { color: white; background: var(--primary); box-shadow: 0 8px 17px rgba(101,87,245,.22); }
    .btn-primary:hover { background: var(--primary-dark); }
    .btn-quiet { color: var(--primary-dark); background: #eeedff; }
    .btn-white { color: var(--ink); background: white; border: 1px solid var(--line); }
    .btn-small { padding: 8px 11px; font-size: 13px; }

    .hero {
      display: grid; grid-template-columns: 1.12fr .88fr; gap: 25px; align-items: stretch;
      padding: 36px; color: white; overflow: hidden; position: relative; border-radius: 30px;
      background: linear-gradient(125deg, #4539bb 0%, #6557f5 55%, #7f75ff 100%);
      box-shadow: var(--shadow);
    }
    .hero::after {
      content: ""; width: 360px; height: 360px; position: absolute; right: -105px; bottom: -170px;
      border: 55px solid rgba(255,255,255,.11); border-radius: 50%;
    }
    .hero-copy, .hero-art { position: relative; z-index: 1; }
    .eyebrow { margin: 0 0 10px; color: #d9d5ff; font-weight: 900; letter-spacing: .09em; text-transform: uppercase; font-size: 12px; }
    h1, h2, h3, p { margin-top: 0; }
    h1 { margin-bottom: 13px; font-size: clamp(32px, 4vw, 53px); line-height: 1.02; letter-spacing: -.06em; }
    .hero-copy > p { max-width: 590px; color: #e4e2ff; font-size: 17px; }
    .hero-stats { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 25px; }
    .hero-stat { padding: 9px 12px; border: 1px solid rgba(255,255,255,.2); border-radius: 12px; color: #f5f4ff; background: rgba(255,255,255,.12); font-size: 13px; }
    .hero-stat strong { display: block; color: white; font-size: 17px; }
    .hero-art { display: grid; place-items: center; min-height: 235px; }
    .hero-cube { width: min(310px, 90%); filter: drop-shadow(0 22px 16px rgba(24, 18, 92, .25)); animation: float 5s ease-in-out infinite; }
    @keyframes float { 0%,100% { transform: translateY(4px) rotate(-2deg); } 50% { transform: translateY(-7px) rotate(2deg); } }

    .section { margin-top: 25px; }
    .section-heading { display: flex; align-items: end; justify-content: space-between; gap: 14px; margin-bottom: 14px; }
    .section-heading h2 { margin: 0; font-size: 25px; letter-spacing: -.04em; }
    .section-heading p { margin: 3px 0 0; color: var(--muted); }
    .card { border: 1px solid rgba(228,233,245,.9); border-radius: var(--radius); background: var(--card); box-shadow: 0 8px 25px rgba(47,55,105,.05); }

    .concept-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
    .concept-card { padding: 20px; min-height: 155px; }
    .concept-icon { width: 39px; height: 39px; display: grid; place-items: center; margin-bottom: 14px; border-radius: 12px; font-size: 20px; }
    .concept-card:nth-child(1) .concept-icon { color: #4c41c9; background: #eeedff; }
    .concept-card:nth-child(2) .concept-icon { color: #007e78; background: #dff8f5; }
    .concept-card:nth-child(3) .concept-icon { color: #b36813; background: #fff0d9; }
    .concept-card h3 { margin-bottom: 6px; font-size: 17px; }
    .concept-card p { margin: 0; color: var(--muted); font-size: 14px; }

    .sim-layout { display: grid; grid-template-columns: 360px 1fr; gap: 18px; align-items: start; }
    .controls { padding: 22px; position: sticky; top: 14px; }
    .controls h3 { margin-bottom: 4px; }
    .controls-intro { color: var(--muted); font-size: 13px; margin-bottom: 18px; }
    .control-row { margin: 17px 0; }
    .control-label { display: flex; justify-content: space-between; align-items: center; gap: 10px; margin-bottom: 8px; font-weight: 800; }
    .control-label span { color: var(--muted); font-size: 13px; font-weight: 600; }
    .range-line { display: grid; grid-template-columns: 1fr 70px; align-items: center; gap: 10px; }
    input[type="range"] {
      width: 100%; height: 7px; appearance: none; border-radius: 10px; background: linear-gradient(90deg, var(--primary) 50%, #e6e9f5 50%);
    }
    input[type="range"]::-webkit-slider-thumb {
      appearance: none; width: 20px; height: 20px; border: 3px solid white; border-radius: 50%;
      background: var(--primary); box-shadow: 0 2px 8px rgba(50,44,150,.3);
    }
    input[type="range"]::-moz-range-thumb { width: 16px; height: 16px; border: 3px solid white; border-radius: 50%; background: var(--primary); }
    .number-input, .activity-input, select {
      width: 100%; border: 1px solid var(--line); border-radius: 10px; padding: 9px 10px;
      color: var(--ink); background: #fbfcff; font-weight: 800;
    }
    .quick-values { display: flex; gap: 7px; flex-wrap: wrap; margin-top: 17px; padding-top: 16px; border-top: 1px solid var(--line); }
    .quick-values .btn { padding: 7px 10px; color: var(--muted); background: #f3f5fb; font-size: 12px; }
    .quick-values .btn:hover { color: var(--primary-dark); background: #eeedff; }

    .visual-column { display: grid; gap: 18px; }
    .visual-card { min-height: 408px; padding: 16px; position: relative; overflow: hidden; background: linear-gradient(145deg, #fcfdff, #f4f5ff); }
    .visual-toolbar { display: flex; justify-content: space-between; align-items: center; gap: 10px; padding: 3px 5px 0; }
    .visual-toolbar strong { font-size: 14px; }
    .visual-toolbar span { color: var(--muted); font-size: 12px; }
    #prismSvg { width: 100%; height: 345px; display: block; }
    .svg-label { font: 800 14px Inter, sans-serif; fill: var(--ink); }
    .svg-measure { font: 800 13px Inter, sans-serif; fill: var(--primary-dark); }

    .metrics { display: grid; grid-template-columns: repeat(4, 1fr); gap: 11px; }
    .metric { padding: 16px; border-radius: 17px; background: white; border: 1px solid var(--line); }
    .metric-label { color: var(--muted); font-size: 12px; font-weight: 700; }
    .metric-value { margin-top: 4px; font-size: 22px; letter-spacing: -.04em; font-weight: 900; }
    .metric:nth-child(1) .metric-value { color: var(--primary); }
    .metric:nth-child(2) .metric-value { color: var(--teal); }
    .metric:nth-child(3) .metric-value { color: var(--orange); }
    .metric:nth-child(4) .metric-value { color: var(--pink); }

    .lower-grid { display: grid; grid-template-columns: 1.1fr .9fr; gap: 18px; }
    .net-card, .formula-card { padding: 22px; }
    .card-title { display: flex; justify-content: space-between; align-items: center; gap: 10px; margin-bottom: 13px; }
    .card-title h3 { margin: 0; font-size: 18px; }
    .pill { display: inline-flex; align-items: center; gap: 5px; border-radius: 99px; padding: 6px 9px; color: #007e78; background: #e0faf7; font-size: 11px; font-weight: 900; }
    #netSvg { width: 100%; height: 215px; display: block; border-radius: 15px; background: #fbfcff; }
    .formula-box { margin: 12px 0; padding: 13px; border-radius: 13px; background: #f5f3ff; }
    .formula-box:last-child { margin-bottom: 0; background: #eafaf7; }
    .formula-name { color: var(--muted); font-size: 12px; font-weight: 800; }
    .formula-line { margin-top: 3px; font-size: 16px; font-weight: 900; }
    .formula-sub { color: var(--muted); font-size: 12px; }

    .example-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
    .example { padding: 19px; position: relative; }
    .example-number { width: 28px; height: 28px; display: grid; place-items: center; margin-bottom: 12px; border-radius: 9px; color: white; background: var(--pink); font-weight: 900; }
    .example:nth-child(2) .example-number { background: var(--teal); }
    .example:nth-child(3) .example-number { background: var(--orange); }
    .example h3 { margin-bottom: 6px; font-size: 16px; }
    .example p { min-height: 65px; margin-bottom: 13px; color: var(--muted); font-size: 14px; }
    .example-answer { padding-top: 12px; border-top: 1px dashed var(--line); font-size: 14px; }
    .example-answer strong { color: var(--primary-dark); }

    .practice-card { padding: 25px; color: white; background: linear-gradient(120deg, #17213b, #26355b); }
    .practice-head { display: flex; justify-content: space-between; align-items: start; gap: 16px; }
    .practice-head h2 { margin-bottom: 5px; color: white; }
    .practice-head p { margin-bottom: 0; color: #b9c5e4; }
    .difficulty-wrap { min-width: 145px; }
    .difficulty-wrap label { display: block; margin-bottom: 5px; color: #b9c5e4; font-size: 12px; font-weight: 700; }
    .difficulty-wrap select { color: var(--ink); background: white; }
    .challenge { margin-top: 20px; padding: 18px; border-radius: 17px; color: var(--ink); background: white; }
    .challenge-tag { color: var(--primary-dark); font-size: 11px; font-weight: 900; letter-spacing: .08em; text-transform: uppercase; }
    #challengeText { margin: 5px 0 16px; font-size: 17px; font-weight: 750; }
    .challenge-form { display: grid; grid-template-columns: 1fr 1fr auto; gap: 10px; align-items: end; }
    .input-label { display: block; margin-bottom: 5px; color: var(--muted); font-size: 12px; font-weight: 800; }
    .feedback { min-height: 24px; margin: 13px 0 0; font-size: 14px; font-weight: 800; }
    .feedback.good { color: var(--green); }
    .feedback.bad { color: var(--danger); }

    .progress-card { display: flex; align-items: center; gap: 18px; padding: 19px 22px; }
    .score-orb { flex: 0 0 auto; width: 66px; height: 66px; display: grid; place-items: center; border-radius: 50%; color: white; background: linear-gradient(135deg, var(--primary), var(--pink)); font-size: 20px; font-weight: 900; }
    .progress-info { flex: 1; }
    .progress-info h3 { margin-bottom: 4px; font-size: 17px; }
    .progress-info p { margin-bottom: 8px; color: var(--muted); font-size: 13px; }
    .progress-track { height: 9px; overflow: hidden; border-radius: 99px; background: #e9ecf7; }
    #progressBar { width: 0%; height: 100%; border-radius: inherit; background: linear-gradient(90deg, var(--teal), var(--primary)); transition: width .35s ease; }
    .badge-list { display: flex; gap: 8px; }
    .badge { width: 39px; height: 39px; display: grid; place-items: center; border-radius: 12px; color: #aab1c7; background: #f0f2f8; filter: grayscale(1); opacity: .52; transition: all .3s ease; }
    .badge.unlocked { color: #ad650e; background: #fff0d6; filter: none; opacity: 1; transform: scale(1.08); }

    .footer { padding-top: 25px; color: var(--muted); text-align: center; font-size: 12px; }

    /* ---------- Ventana emergente ---------- */
    .modal-backdrop { position: fixed; inset: 0; display: none; place-items: center; padding: 18px; background: rgba(18, 23, 48, .55); z-index: 5; }
    .modal-backdrop.open { display: grid; }
    .modal { width: min(450px, 100%); padding: 25px; border-radius: 22px; background: white; box-shadow: var(--shadow); animation: appear .22s ease; }
    @keyframes appear { from { opacity: 0; transform: translateY(10px) scale(.98); } to { opacity: 1; transform: none; } }
    .modal h2 { margin-bottom: 8px; }
    .modal p { color: var(--muted); }
    .modal-actions { display: flex; justify-content: end; gap: 8px; margin-top: 18px; }

    @media (max-width: 920px) {
      .hero, .sim-layout, .lower-grid { grid-template-columns: 1fr; }
      .controls { position: static; }
      .hero-art { min-height: 175px; }
    }
    @media (max-width: 650px) {
      .app-shell { padding: 14px 13px 35px; }
      .topbar { margin-bottom: 14px; }
      .top-actions .btn-quiet { display: none; }
      .hero { padding: 26px 21px; border-radius: 23px; }
      .hero-art { min-height: 140px; }
      .concept-grid, .example-grid, .metrics { grid-template-columns: 1fr 1fr; }
      .concept-card:last-child, .example:last-child { grid-column: 1 / -1; }
      .visual-card { min-height: 330px; }
      #prismSvg { height: 285px; }
      .challenge-form { grid-template-columns: 1fr 1fr; }
      .challenge-form .btn { grid-column: 1 / -1; }
      .progress-card { flex-wrap: wrap; }
      .progress-info { min-width: calc(100% - 84px); }
      .badge-list { width: 100%; justify-content: center; }
    }
    @media (max-width: 420px) {
      .metrics { grid-template-columns: 1fr 1fr; }
      .section-heading { display: block; }
      .section-heading p { margin-top: 4px; }
    }
  </style>
</head>
<body>
  <main class="app-shell">
    <header class="topbar">
      <div class="brand" aria-label="PrismaLab">
        <div class="brand-mark" aria-hidden="true">◇</div>
        <div>PrismaLab<small>Laboratorio de geometría</small></div>
      </div>
      <div class="top-actions">
        <button class="btn btn-quiet btn-small" id="hintBtn">💡 Pista</button>
        <button class="btn btn-white btn-small" id="resetBtn">↻ Reiniciar</button>
      </div>
    </header>

    <!-- Pantalla de bienvenida -->
    <section class="hero" aria-labelledby="welcomeTitle">
      <div class="hero-copy">
        <p class="eyebrow">Simulador interactivo · Nivel secundaria</p>
        <h1 id="welcomeTitle">Explora el mundo de los prismas.</h1>
        <p>Mueve las dimensiones, observa cómo cambia el sólido y descubre la relación entre sus medidas, el área y el volumen.</p>
        <div class="hero-stats">
          <div class="hero-stat"><strong>3D</strong>Vista dinámica</div>
          <div class="hero-stat"><strong>2 retos</strong>Para practicar</div>
          <div class="hero-stat"><strong>∞</strong>Experimentos</div>
        </div>
      </div>
      <div class="hero-art" aria-hidden="true">
        <svg class="hero-cube" viewBox="0 0 320 240">
          <polygon points="70,75 170,30 268,77 168,126" fill="#aaa4ff"/>
          <polygon points="70,75 168,126 168,213 70,162" fill="#7167ed"/>
          <polygon points="168,126 268,77 268,164 168,213" fill="#5045c7"/>
          <path d="M70 75L168 126L268 77M168 126v87M70 75v87l98 51 100-49V77L170 30 70 75Z" fill="none" stroke="#fff" stroke-width="3" stroke-linejoin="round"/>
          <path d="M42 190h96M209 218h72M161 15v215" fill="none" stroke="rgba(255,255,255,.3)" stroke-width="2" stroke-dasharray="5 7"/>
        </svg>
      </div>
    </section>

    <!-- Explicación breve -->
    <section class="section" aria-labelledby="conceptTitle">
      <div class="section-heading">
        <div><h2 id="conceptTitle">Tres ideas para comenzar</h2><p>Un prisma tiene dos bases iguales y paralelas.</p></div>
      </div>
      <div class="concept-grid">
        <article class="card concept-card">
          <div class="concept-icon">▣</div>
          <h3>Área de la base</h3>
          <p>En un prisma rectangular, la base es un rectángulo: <strong>largo × ancho</strong>.</p>
        </article>
        <article class="card concept-card">
          <div class="concept-icon">↕</div>
          <h3>Altura</h3>
          <p>Es la distancia perpendicular entre las dos bases. Aquí cambia la profundidad del sólido.</p>
        </article>
        <article class="card concept-card">
          <div class="concept-icon">◈</div>
          <h3>Volumen</h3>
          <p>El espacio que ocupa se calcula con <strong>área de la base × altura</strong>.</p>
        </article>
      </div>
    </section>

    <!-- Zona de simulación y controles dinámicos -->
    <section class="section" aria-labelledby="simulationTitle">
      <div class="section-heading">
        <div><h2 id="simulationTitle">Construye tu prisma</h2><p>Cambia una medida y observa la transformación en tiempo real.</p></div>
      </div>
      <div class="sim-layout">
        <aside class="card controls" aria-label="Controles de dimensiones">
          <h3>Dimensiones</h3>
          <p class="controls-intro">Usa los deslizadores o escribe un valor entre 1 y 12.</p>

          <div class="control-row">
            <div class="control-label"><label for="lengthRange">Largo <span>l</span></label><span id="lengthHint">cm</span></div>
            <div class="range-line"><input id="lengthRange" type="range" min="1" max="12" step=".5" value="6" aria-label="Largo del prisma" /><input id="lengthNumber" class="number-input" type="number" min="1" max="12" step=".5" value="6" aria-label="Largo numérico" /></div>
          </div>
          <div class="control-row">
            <div class="control-label"><label for="widthRange">Ancho <span>a</span></label><span>cm</span></div>
            <div class="range-line"><input id="widthRange" type="range" min="1" max="12" step=".5" value="4" aria-label="Ancho del prisma" /><input id="widthNumber" class="number-input" type="number" min="1" max="12" step=".5" value="4" aria-label="Ancho numérico" /></div>
          </div>
          <div class="control-row">
            <div class="control-label"><label for="heightRange">Altura <span>h</span></label><span>cm</span></div>
            <div class="range-line"><input id="heightRange" type="range" min="1" max="12" step=".5" value="5" aria-label="Altura del prisma" /><input id="heightNumber" class="number-input" type="number" min="1" max="12" step=".5" value="5" aria-label="Altura numérica" /></div>
          </div>
          <div class="quick-values" aria-label="Tamaños rápidos">
            <span style="width:100%; color:var(--muted); font-size:12px; font-weight:800;">Probar medidas:</span>
            <button class="btn" data-preset="4,3,2">Pequeño</button>
            <button class="btn" data-preset="6,4,5">Mediano</button>
            <button class="btn" data-preset="10,7,8">Grande</button>
          </div>
        </aside>

        <div class="visual-column">
          <div class="card visual-card">
            <div class="visual-toolbar"><strong>Vista pseudo 3D</strong><span id="dimensionCaption">6 × 4 × 5 cm</span></div>
            <!-- SVG: se actualiza desde JavaScript para dibujar el prisma y sus cotas -->
            <svg id="prismSvg" viewBox="0 0 720 350" role="img" aria-label="Representación tridimensional de un prisma rectangular">
              <defs>
                <linearGradient id="frontGradient" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#8177ff"/><stop offset="1" stop-color="#5b50db"/></linearGradient>
                <linearGradient id="topGradient" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#c1bcff"/><stop offset="1" stop-color="#928aff"/></linearGradient>
                <linearGradient id="sideGradient" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#5c52dc"/><stop offset="1" stop-color="#4037a9"/></linearGradient>
              </defs>
              <ellipse id="shadowEllipse" cx="360" cy="294" rx="180" ry="20" fill="rgba(72,62,175,.12)"/>
              <g id="prismGroup">
                <polygon id="prismTop" fill="url(#topGradient)" stroke="#fff" stroke-width="3" stroke-linejoin="round"/>
                <polygon id="prismFront" fill="url(#frontGradient)" stroke="#fff" stroke-width="3" stroke-linejoin="round"/>
                <polygon id="prismSide" fill="url(#sideGradient)" stroke="#fff" stroke-width="3" stroke-linejoin="round"/>
                <line id="depthDashed" stroke="rgba(255,255,255,.7)" stroke-width="2" stroke-dasharray="7 6"/>
              </g>
              <g id="measureLines" fill="none" stroke="#6557f5" stroke-width="2">
                <path id="lengthMeasure"/><path id="widthMeasure"/><path id="heightMeasure"/>
              </g>
              <g id="measureLabels" text-anchor="middle">
                <text id="lengthLabel" class="svg-measure"></text><text id="widthLabel" class="svg-measure"></text><text id="heightLabel" class="svg-measure"></text>
              </g>
              <text id="solidLabel" x="360" y="45" text-anchor="middle" class="svg-label">Prisma rectangular</text>
            </svg>
          </div>
          <div class="metrics" aria-live="polite">
            <div class="metric"><div class="metric-label">Área de la base</div><div class="metric-value" id="baseAreaValue">24 cm²</div></div>
            <div class="metric"><div class="metric-label">Volumen</div><div class="metric-value" id="volumeValue">120 cm³</div></div>
            <div class="metric"><div class="metric-label">Área total</div><div class="metric-value" id="surfaceValue">148 cm²</div></div>
            <div class="metric"><div class="metric-label">Diagonal</div><div class="metric-value" id="diagonalValue">8.77 cm</div></div>
          </div>
        </div>
      </div>
    </section>

    <!-- Visualización de desarrollo plano y fórmulas -->
    <section class="section lower-grid" aria-label="Desarrollo plano y fórmulas">
      <article class="card net-card">
        <div class="card-title"><h3>Desarrollo plano</h3><span class="pill">▣ 6 caras</span></div>
        <p style="color:var(--muted);font-size:13px;">Así se verían todas las caras del prisma extendidas.</p>
        <svg id="netSvg" viewBox="0 0 600 215" role="img" aria-label="Desarrollo plano del prisma">
          <g id="netGroup" stroke="#fff" stroke-width="3" stroke-linejoin="round"></g>
          <g id="netLabels" fill="#4c41c9" font-family="Inter, sans-serif" font-size="12" font-weight="800" text-anchor="middle"></g>
        </svg>
      </article>
      <article class="card formula-card">
        <div class="card-title"><h3>Fórmulas en acción</h3><span class="pill">Paso a paso</span></div>
        <div class="formula-box"><div class="formula-name">Área de la base</div><div class="formula-line" id="formulaBase">A<sub>b</sub> = 6 × 4 = 24 cm²</div></div>
        <div class="formula-box"><div class="formula-name">Volumen</div><div class="formula-line" id="formulaVolume">V = A<sub>b</sub> × h = 24 × 5 = 120 cm³</div><div class="formula-sub">base × altura</div></div>
        <div class="formula-box"><div class="formula-name">Área total</div><div class="formula-line" id="formulaSurface">A<sub>t</sub> = 2(6×4 + 6×5 + 4×5)</div><div class="formula-sub" id="formulaSurfaceResult">= 148 cm²</div></div>
      </article>
    </section>

    <!-- Ejemplos guiados -->
    <section class="section" aria-labelledby="examplesTitle">
      <div class="section-heading"><div><h2 id="examplesTitle">Ejemplos guiados</h2><p>Conecta las fórmulas con situaciones del día a día.</p></div></div>
      <div class="example-grid">
        <article class="card example">
          <div class="example-number">1</div><h3>Una caja de regalo</h3>
          <p>Una caja mide 8 cm de largo, 5 cm de ancho y 3 cm de alto. ¿Cuánto espacio hay dentro?</p>
          <div class="example-answer">Volumen: <strong>8 × 5 × 3 = 120 cm³</strong></div>
        </article>
        <article class="card example">
          <div class="example-number">2</div><h3>Una pecera</h3>
          <p>Si duplicas el largo y mantienes lo demás, la base también se duplica. ¿Qué ocurre con el volumen?</p>
          <div class="example-answer">El volumen <strong>también se duplica</strong>.</div>
        </article>
        <article class="card example">
          <div class="example-number">3</div><h3>Forrar un paquete</h3>
          <p>Para saber cuánto papel necesitas, calcula el área de las seis caras, no el volumen.</p>
          <div class="example-answer">Se usa el <strong>área total</strong>: 2(la + lh + ah).</div>
        </article>
      </div>
    </section>

    <!-- Actividad práctica y retroalimentación -->
    <section class="section card practice-card" aria-labelledby="practiceTitle">
      <div class="practice-head">
        <div><h2 id="practiceTitle">Desafío del laboratorio</h2><p>Resuelve el reto y gana puntos para desbloquear insignias.</p></div>
        <div class="difficulty-wrap"><label for="difficulty">Dificultad</label><select id="difficulty"><option value="easy">Explorador</option><option value="medium">Constructor</option><option value="hard">Arquitecto</option></select></div>
      </div>
      <div class="challenge">
        <div class="challenge-tag">Reto activo</div>
        <div id="challengeText">Calcula el volumen de un prisma de 5 cm × 3 cm × 4 cm.</div>
        <div class="challenge-form">
          <div><label class="input-label" for="answerInput">Tu respuesta</label><input id="answerInput" class="activity-input" type="number" min="0" step=".01" placeholder="Escribe el resultado" /></div>
          <div><label class="input-label" for="answerUnit">Unidad</label><select id="answerUnit"><option value="volume">cm³ (volumen)</option><option value="area">cm² (área total)</option></select></div>
          <button class="btn btn-primary" id="checkAnswer">Comprobar respuesta →</button>
        </div>
        <div class="feedback" id="feedback" aria-live="polite"></div>
      </div>
    </section>

    <!-- Sistema de puntuación e insignias -->
    <section class="section card progress-card">
      <div class="score-orb" id="scoreValue">0</div>
      <div class="progress-info">
        <h3>Tu progreso</h3>
        <p id="progressText">Consigue 50 puntos para desbloquear tu primera insignia.</p>
        <div class="progress-track" aria-label="Progreso hacia la siguiente insignia"><div id="progressBar"></div></div>
      </div>
      <div class="badge-list" aria-label="Insignias">
        <div class="badge" id="badge1" title="Explorador: 50 puntos">🔎</div>
        <div class="badge" id="badge2" title="Constructor: 100 puntos">🧱</div>
        <div class="badge" id="badge3" title="Arquitecto: 150 puntos">🏆</div>
      </div>
    </section>

    <footer class="footer">PrismaLab · Aprende haciendo · Todos los cálculos se realizan en tu navegador.</footer>
  </main>

  <!-- Ventana emergente educativa -->
  <div class="modal-backdrop" id="modalBackdrop" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
    <div class="modal">
      <h2 id="modalTitle">Pista rápida</h2>
      <p id="modalText">El volumen de un prisma rectangular se obtiene multiplicando largo × ancho × altura.</p>
      <div class="modal-actions"><button class="btn btn-primary" id="closeModal">Entendido</button></div>
    </div>
  </div>

  <script>
    /* ---------- Estado y utilidades ---------- */
    const state = { length: 6, width: 4, height: 5, score: 0, challenge: null };
    const $ = (id) => document.getElementById(id);
    const fmt = (n) => Number.isInteger(n) ? String(n) : n.toFixed(2).replace(/\.?0+$/, "");
    const clamp = (n, min, max) => Math.min(max, Math.max(min, n));

    // Actualiza una pareja de controles (slider + campo numérico).
    function bindDimension(name) {
      const range = $(`${name}Range`);
      const number = $(`${name}Number`);
      const update = (source) => {
        let value = parseFloat(source.value);
        if (!Number.isFinite(value)) value = state[name];
        value = clamp(value, 1, 12);
        state[name] = value;
        range.value = value;
        number.value = value;
        const percent = ((value - 1) / 11) * 100;
        range.style.background = `linear-gradient(90deg, var(--primary) ${percent}%, #e6e9f5 ${percent}%)`;
        render();
      };
      range.addEventListener("input", () => update(range));
      number.addEventListener("input", () => update(number));
    }

    // Dibuja el prisma con caras proporcionales y etiquetas de medida.
    function renderPrism() {
      const l = state.length, w = state.width, h = state.height;
      const depth = 31 + w * 2.6;
      const width = 190 + l * 17;
      const height = 92 + h * 11;
      const x = 360 - width / 2;
      const y = 110;
      const dx = depth * .85, dy = -depth * .46;
      const front = `${x},${y} ${x + width},${y} ${x + width},${y + height} ${x},${y + height}`;
      const top = `${x},${y} ${x + dx},${y + dy} ${x + width + dx},${y + dy} ${x + width},${y}`;
      const side = `${x + width},${y} ${x + width + dx},${y + dy} ${x + width + dx},${y + height + dy} ${x + width},${y + height}`;
      $("prismFront").setAttribute("points", front);
      $("prismTop").setAttribute("points", top);
      $("prismSide").setAttribute("points", side);
      $("depthDashed").setAttribute("x1", x + dx); $("depthDashed").setAttribute("y1", y + dy);
      $("depthDashed").setAttribute("x2", x + dx); $("depthDashed").setAttribute("y2", y + height + dy);
      $("shadowEllipse").setAttribute("cx", x + width / 2 + dx / 2);
      $("shadowEllipse").setAttribute("cy", y + height + 23);
      $("shadowEllipse").setAttribute("rx", Math.max(115, width * .57));
      $("shadowEllipse").setAttribute("ry", 15 + w * .8);

      $("lengthMeasure").setAttribute("d", `M${x},${y + height + 18} V${y + height + 31} H${x + width} V${y + height + 18}`);
      $("widthMeasure").setAttribute("d", `M${x + width + 11},${y - 3} l${dx},${dy} M${x + width + 5},${y - 9} l${dx},${dy}`);
      $("heightMeasure").setAttribute("d", `M${x - 19},${y} H${x - 32} V${y + height} H${x - 19}`);
      $("lengthLabel").setAttribute("x", x + width / 2); $("lengthLabel").setAttribute("y", y + height + 51); $("lengthLabel").textContent = `l = ${fmt(l)} cm`;
      $("widthLabel").setAttribute("x", x + width + dx / 2 + 19); $("widthLabel").setAttribute("y", y + dy / 2 - 4); $("widthLabel").textContent = `a = ${fmt(w)} cm`;
      $("heightLabel").setAttribute("x", x - 47); $("heightLabel").setAttribute("y", y + height / 2 + 5); $("heightLabel").textContent = `h = ${fmt(h)} cm`;
    }

    // Dibuja el desarrollo plano con seis rectángulos a escala.
    function renderNet() {
      const l = state.length, w = state.width, h = state.height;
      const unit = Math.min(20, 125 / Math.max(l, w, h));
      const bw = l * unit, bh = w * unit, sh = h * unit;
      const cx = 300, cy = 108;
      const faces = [
        { x: cx - bw / 2, y: cy - bh / 2, width: bw, height: bh, color: "#8278ff", label: "base" },
        { x: cx - bw / 2, y: cy - bh / 2 - sh, width: bw, height: sh, color: "#aaa4ff", label: "lado" },
        { x: cx - bw / 2, y: cy + bh / 2, width: bw, height: sh, color: "#aaa4ff", label: "lado" },
        { x: cx - bw / 2 - sh, y: cy - bh / 2, width: sh, height: bh, color: "#6358df", label: "lado" },
        { x: cx + bw / 2, y: cy - bh / 2, width: sh, height: bh, color: "#6358df", label: "lado" },
        { x: cx - bw / 2, y: cy + bh / 2 + sh, width: bw, height: bh, color: "#8278ff", label: "base" }
      ];
      $("netGroup").innerHTML = faces.map(f => `<rect x="${f.x}" y="${f.y}" width="${f.width}" height="${f.height}" rx="3" fill="${f.color}"/>`).join("");
      $("netLabels").innerHTML = faces.map(f => `<text x="${f.x + f.width / 2}" y="${f.y + f.height / 2 + 4}">${f.label}</text>`).join("");
    }

    // Calcula y muestra todas las magnitudes derivadas.
    function render() {
      const { length: l, width: w, height: h } = state;
      const base = l * w, volume = base * h, surface = 2 * (l * w + l * h + w * h);
      const diagonal = Math.sqrt(l * l + w * w + h * h);
      $("dimensionCaption").textContent = `${fmt(l)} × ${fmt(w)} × ${fmt(h)} cm`;
      $("baseAreaValue").textContent = `${fmt(base)} cm²`;
      $("volumeValue").textContent = `${fmt(volume)} cm³`;
      $("surfaceValue").textContent = `${fmt(surface)} cm²`;
      $("diagonalValue").textContent = `${fmt(diagonal)} cm`;
      $("formulaBase").innerHTML = `A<sub>b</sub> = ${fmt(l)} × ${fmt(w)} = ${fmt(base)} cm²`;
      $("formulaVolume").innerHTML = `V = A<sub>b</sub> × h = ${fmt(base)} × ${fmt(h)} = ${fmt(volume)} cm³`;
      $("formulaSurface").innerHTML = `A<sub>t</sub> = 2(${fmt(l)}×${fmt(w)} + ${fmt(l)}×${fmt(h)} + ${fmt(w)}×${fmt(h)})`;
      $("formulaSurfaceResult").textContent = `= ${fmt(surface)} cm²`;
      renderPrism(); renderNet();
    }

    /* ---------- Actividad y gamificación ---------- */
    function makeChallenge() {
      const difficulty = $("difficulty").value;
      const max = difficulty === "easy" ? 6 : difficulty === "medium" ? 9 : 12;
      const a = Math.ceil(Math.random() * (max - 2)) + 2;
      const b = Math.ceil(Math.random() * (max - 2)) + 2;
      const c = Math.ceil(Math.random() * (max - 2)) + 2;
      const type = difficulty === "easy" || Math.random() < .65 ? "volume" : "area";
      const answer = type === "volume" ? a * b * c : 2 * (a * b + a * c + b * c);
      state.challenge = { a, b, c, type, answer };
      $("answerUnit").value = type;
      $("challengeText").textContent = type === "volume"
        ? `Calcula el volumen de un prisma de ${a} cm × ${b} cm × ${c} cm.`
        : `Calcula el área total de un prisma de ${a} cm × ${b} cm × ${c} cm.`;
      $("answerInput").value = "";
      $("feedback").textContent = "";
      $("feedback").className = "feedback";
    }

    function checkAnswer() {
      const value = parseFloat($("answerInput").value);
      const unit = $("answerUnit").value;
      const challenge = state.challenge;
      if (!Number.isFinite(value)) {
        $("feedback").textContent = "Escribe un número para comprobar tu respuesta.";
        $("feedback").className = "feedback bad";
        return;
      }
      if (unit !== challenge.type) {
        $("feedback").textContent = "Revisa la unidad: este reto pide " + (challenge.type === "volume" ? "volumen (cm³)." : "área total (cm²).");
        $("feedback").className = "feedback bad";
        return;
      }
      if (Math.abs(value - challenge.answer) < .01) {
        const points = $("difficulty").value === "easy" ? 25 : $("difficulty").value === "medium" ? 40 : 60;
        state.score += points;
        $("feedback").textContent = `¡Excelente! ${challenge.type === "volume" ? "Multiplicaste base × altura." : "Sumaste las seis caras."} +${points} puntos.`;
        $("feedback").className = "feedback good";
        updateScore();
        setTimeout(makeChallenge, 900);
      } else {
        $("feedback").textContent = "Aún no. Pista: " + (challenge.type === "volume" ? "multiplica las tres dimensiones." : "usa 2(la + lh + ah).");
        $("feedback").className = "feedback bad";
      }
    }

    function updateScore() {
      const score = state.score;
      $("scoreValue").textContent = score;
      const next = score < 50 ? 50 : score < 100 ? 100 : score < 150 ? 150 : 150;
      $("progressBar").style.width = `${Math.min(100, (score / next) * 100)}%`;
      $("progressText").textContent = score >= 150 ? "¡Nivel Arquitecto desbloqueado! Dominas el laboratorio." : `Te faltan ${Math.max(0, next - score)} puntos para la siguiente insignia.`;
      $("badge1").classList.toggle("unlocked", score >= 50);
      $("badge2").classList.toggle("unlocked", score >= 100);
      $("badge3").classList.toggle("unlocked", score >= 150);
    }

    /* ---------- Eventos ---------- */
    ["length", "width", "height"].forEach(bindDimension);
    document.querySelectorAll("[data-preset]").forEach(button => {
      button.addEventListener("click", () => {
        const [l, w, h] = button.dataset.preset.split(",").map(Number);
        state.length = l; state.width = w; state.height = h;
        ["length", "width", "height"].forEach(name => {
          $(`${name}Range`).value = state[name];
          $(`${name}Number`).value = state[name];
        });
        render();
      });
    });
    $("checkAnswer").addEventListener("click", checkAnswer);
    $("answerInput").addEventListener("keydown", (event) => { if (event.key === "Enter") checkAnswer(); });
    $("difficulty").addEventListener("change", makeChallenge);
    $("resetBtn").addEventListener("click", () => {
      state.length = 6; state.width = 4; state.height = 5; state.score = 0;
      ["length", "width", "height"].forEach(name => { $(`${name}Range`).value = state[name]; $(`${name}Number`).value = state[name]; });
      render(); updateScore(); makeChallenge();
    });

    // Pista contextual: cambia según el volumen actual del simulador.
    $("hintBtn").addEventListener("click", () => {
      const volume = state.length * state.width * state.height;
      $("modalText").textContent = `Observa el prisma actual: su volumen es ${fmt(volume)} cm³. Para cualquier prisma rectangular, multiplica largo × ancho × altura.`;
      $("modalBackdrop").classList.add("open");
      $("closeModal").focus();
    });
    $("closeModal").addEventListener("click", () => $("modalBackdrop").classList.remove("open"));
    $("modalBackdrop").addEventListener("click", (event) => { if (event.target === $("modalBackdrop")) $("modalBackdrop").classList.remove("open"); });
    document.addEventListener("keydown", (event) => { if (event.key === "Escape") $("modalBackdrop").classList.remove("open"); });

    // Primer renderizado.
    render();
    makeChallenge();
    updateScore();
  </script>
</body>
</html>
