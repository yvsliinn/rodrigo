<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EcoBriq — Prototipo Interactivo</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;700&family=Barlow:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0e0f0e;
    --bg2: #161917;
    --bg3: #1e2220;
    --surface: #242824;
    --surface2: #2d322d;
    --border: #3a403a;
    --border2: #4d564d;
    --accent: #7ab648;
    --accent2: #5d8f35;
    --accent3: #9fd063;
    --steel: #8a9b8a;
    --text: #e8ede8;
    --text2: #aab8aa;
    --text3: #6d7d6d;
    --highlight: #c8e89a;
    --orange: #d4883c;
    --amber: #c47a28;
    --rust: #8b4513;
  }

  * { margin:0; padding:0; box-sizing:border-box; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Barlow', sans-serif;
    font-weight: 300;
    min-height: 100vh;
  }

  header {
    background: var(--bg2);
    border-bottom: 1px solid var(--border);
    padding: 1.2rem 3rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 2rem;
    font-weight: 700;
    color: var(--accent);
    letter-spacing: 0.02em;
  }
  .logo span { color: var(--text2); font-weight: 400; font-size: 0.9rem; display:block; letter-spacing: 0.15em; text-transform: uppercase; }

  .tagline {
    font-size: 0.75rem;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--text3);
  }

  .main-wrapper {
    display: grid;
    grid-template-columns: 1fr 380px;
    min-height: calc(100vh - 72px);
  }

  /* LEFT: Machine Diagram */
  .diagram-panel {
    padding: 3rem;
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  .section-label {
    font-size: 0.7rem;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--text3);
    margin-bottom: 0.5rem;
  }

  .diagram-title {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 1.6rem;
    font-weight: 600;
    color: var(--text);
    line-height: 1.2;
  }

  .diagram-subtitle {
    font-size: 0.9rem;
    color: var(--text2);
    margin-top: 0.3rem;
  }

  .machine-container {
    position: relative;
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 4px;
    padding: 2rem;
    flex: 1;
  }

  /* Machine SVG region */
  .machine-svg-wrap {
    position: relative;
    width: 100%;
  }

  .machine-svg-wrap svg {
    width: 100%;
    height: auto;
    display: block;
  }

  /* Clickable hotspots */
  .hotspot {
    position: absolute;
    cursor: pointer;
    border-radius: 50%;
    width: 28px;
    height: 28px;
    background: var(--accent);
    border: 2px solid var(--accent3);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 0.85rem;
    color: #0e0f0e;
    transition: all 0.2s ease;
    z-index: 10;
    transform: translate(-50%, -50%);
    box-shadow: 0 0 0 4px rgba(122,182,72,0.15);
  }

  .hotspot:hover {
    background: var(--accent3);
    box-shadow: 0 0 0 8px rgba(122,182,72,0.25);
    transform: translate(-50%, -50%) scale(1.15);
  }

  .hotspot.active {
    background: var(--highlight);
    box-shadow: 0 0 0 8px rgba(200,232,154,0.3);
    transform: translate(-50%, -50%) scale(1.2);
  }

  /* Process steps bar */
  .process-bar {
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    gap: 2px;
    margin-top: 1.5rem;
  }

  .process-step {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 2px;
    padding: 0.5rem 0.3rem;
    text-align: center;
    cursor: pointer;
    transition: all 0.2s;
    position: relative;
  }

  .process-step:hover {
    background: var(--surface2);
    border-color: var(--accent2);
  }

  .process-step.active {
    background: var(--surface2);
    border-color: var(--accent);
    border-top: 2px solid var(--accent);
  }

  .step-num {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 1rem;
    font-weight: 700;
    color: var(--accent);
    display: block;
  }

  .step-label {
    font-size: 0.6rem;
    color: var(--text3);
    text-transform: uppercase;
    letter-spacing: 0.05em;
    display: block;
    margin-top: 2px;
    line-height: 1.2;
  }

  /* RIGHT: Info Panel */
  .info-panel {
    background: var(--bg2);
    border-left: 1px solid var(--border);
    display: flex;
    flex-direction: column;
  }

  .info-header {
    padding: 2rem;
    border-bottom: 1px solid var(--border);
    background: var(--bg3);
  }

  .info-part-num {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 3rem;
    font-weight: 700;
    color: var(--border2);
    line-height: 1;
    margin-bottom: 0.3rem;
  }

  .info-part-name {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 1.4rem;
    font-weight: 600;
    color: var(--accent3);
    text-transform: uppercase;
    letter-spacing: 0.05em;
  }

  .info-part-subtitle {
    font-size: 0.8rem;
    color: var(--text3);
    margin-top: 0.3rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .info-body {
    padding: 2rem;
    flex: 1;
    overflow-y: auto;
  }

  .info-section {
    margin-bottom: 2rem;
  }

  .info-section-label {
    font-size: 0.65rem;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--text3);
    margin-bottom: 0.6rem;
    padding-bottom: 0.4rem;
    border-bottom: 1px solid var(--border);
  }

  .info-desc {
    font-size: 0.9rem;
    color: var(--text2);
    line-height: 1.7;
  }

  .info-specs {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }

  .spec-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5rem 0;
    border-bottom: 1px solid var(--border);
    font-size: 0.82rem;
  }

  .spec-key {
    color: var(--text3);
  }

  .spec-val {
    color: var(--accent3);
    font-weight: 500;
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 0.95rem;
  }

  .material-tag {
    display: inline-block;
    background: var(--surface2);
    border: 1px solid var(--border2);
    color: var(--text2);
    font-size: 0.72rem;
    padding: 0.25rem 0.7rem;
    border-radius: 2px;
    margin: 0.2rem;
    letter-spacing: 0.05em;
    text-transform: uppercase;
  }

  .info-placeholder {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
    text-align: center;
    gap: 1rem;
    padding: 2rem;
  }

  .placeholder-icon {
    width: 60px;
    height: 60px;
    border: 1px solid var(--border);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto;
  }

  .placeholder-text {
    font-size: 0.85rem;
    color: var(--text3);
    line-height: 1.6;
  }

  /* Bottom metrics */
  .metrics-row {
    padding: 1.5rem 2rem;
    border-top: 1px solid var(--border);
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 1rem;
    background: var(--bg3);
  }

  .metric-card {
    text-align: center;
  }

  .metric-val {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 1.4rem;
    font-weight: 700;
    color: var(--accent);
    display: block;
  }

  .metric-label {
    font-size: 0.65rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--text3);
    display: block;
    margin-top: 2px;
  }

  /* Instruction hint */
  .hint-bar {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 2px;
    padding: 0.7rem 1rem;
    font-size: 0.78rem;
    color: var(--text3);
    display: flex;
    align-items: center;
    gap: 0.6rem;
  }

  .hint-dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--accent);
    flex-shrink: 0;
    animation: pulse 2s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.3; }
  }

  /* Connector lines on process bar */
  .process-step::after {
    content: '';
    position: absolute;
    right: -2px;
    top: 50%;
    width: 2px;
    height: 8px;
    background: var(--border);
    transform: translateY(-50%);
    z-index: 1;
  }
  .process-step:last-child::after { display: none; }

</style>
</head>
<body>

<header>
  <div class="logo">
    EcoBriq
    <span>Sistema de Compactación de Aserrín</span>
  </div>
  <div class="tagline">Prototipo Interactivo — Partes y Funciones</div>
</header>

<div class="main-wrapper">

  <!-- LEFT PANEL -->
  <div class="diagram-panel">
    <div>
      <div class="section-label">Diagrama del sistema</div>
      <div class="diagram-title">Máquina Compactadora de Aserrín</div>
      <div class="diagram-subtitle">Selecciona un componente para ver su función y composición</div>
    </div>

    <div class="hint-bar">
      <div class="hint-dot"></div>
      Haz clic en cualquier número marcado en el diagrama o en los pasos del proceso
    </div>

    <div class="machine-container">
      <div class="machine-svg-wrap" id="svgWrap">

        <!-- Main machine SVG illustration (schematic style) -->
        <svg viewBox="0 0 760 420" fill="none" xmlns="http://www.w3.org/2000/svg">

          <!-- Background grid -->
          <defs>
            <pattern id="grid" width="30" height="30" patternUnits="userSpaceOnUse">
              <path d="M 30 0 L 0 0 0 30" fill="none" stroke="#2a2e2a" stroke-width="0.5"/>
            </pattern>
          </defs>
          <rect width="760" height="420" fill="url(#grid)" rx="2"/>

          <!-- Main machine body frame -->
          <rect x="30" y="80" width="700" height="240" rx="3" fill="#1a1e1a" stroke="#3a403a" stroke-width="1.5"/>
          
          <!-- Machine base platform -->
          <rect x="30" y="310" width="700" height="18" rx="2" fill="#242824" stroke="#4d564d" stroke-width="1"/>
          
          <!-- PART 1: Feeding chute / hopper -->
          <polygon points="60,80 140,80 125,30 75,30" fill="#2d322d" stroke="#5d8f35" stroke-width="2"/>
          <text x="100" y="58" fill="#7ab648" font-family="Barlow Condensed" font-size="10" font-weight="600" text-anchor="middle">TOLVA</text>
          <line x1="75" y1="30" x2="125" y2="30" stroke="#5d8f35" stroke-width="1.5"/>
          <line x1="60" y1="80" x2="75" y2="30" stroke="#5d8f35" stroke-width="1.5"/>
          <line x1="140" y1="80" x2="125" y2="30" stroke="#5d8f35" stroke-width="1.5"/>
          <!-- Sawdust dots in hopper -->
          <circle cx="90" cy="55" r="2" fill="#c47a28" opacity="0.7"/>
          <circle cx="100" cy="65" r="2" fill="#c47a28" opacity="0.6"/>
          <circle cx="110" cy="50" r="2" fill="#c47a28" opacity="0.8"/>
          <circle cx="85" cy="70" r="1.5" fill="#c47a28" opacity="0.5"/>
          <circle cx="115" cy="68" r="1.5" fill="#d4883c" opacity="0.7"/>

          <!-- PART 2: Raw material auger / feed screw -->
          <rect x="60" y="150" width="150" height="40" rx="3" fill="#1e2220" stroke="#4d564d" stroke-width="1.5"/>
          <!-- Auger coil -->
          <path d="M 70,160 Q 85,148 100,160 Q 115,172 130,160 Q 145,148 160,160 Q 175,172 190,160 Q 205,148 210,155" stroke="#7ab648" stroke-width="2.5" fill="none"/>
          <path d="M 70,175 Q 85,163 100,175 Q 115,187 130,175 Q 145,163 160,175 Q 175,187 190,175 Q 205,163 210,170" stroke="#5d8f35" stroke-width="2" fill="none"/>
          <text x="135" y="205" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">TORNILLO SIN FIN</text>

          <!-- PART 3: Drying chamber -->
          <rect x="220" y="130" width="80" height="80" rx="2" fill="#242824" stroke="#d4883c" stroke-width="1.5" stroke-dasharray="4,2"/>
          <!-- Heat wavy lines -->
          <path d="M 235,160 Q 242,152 250,160 Q 257,168 265,160 Q 272,152 280,160" stroke="#d4883c" stroke-width="1.5" fill="none"/>
          <path d="M 235,170 Q 242,162 250,170 Q 257,178 265,170 Q 272,162 280,170" stroke="#c47a28" stroke-width="1.5" fill="none"/>
          <path d="M 235,180 Q 242,172 250,180 Q 257,188 265,180 Q 272,172 280,180" stroke="#9d5e1c" stroke-width="1" fill="none"/>
          <text x="260" y="225" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">CÁMARA SECADO</text>
          <!-- Temp indicator -->
          <rect x="290" y="145" width="4" height="50" rx="2" fill="#3a403a"/>
          <rect x="290" y="165" width="4" height="30" rx="2" fill="#d4883c"/>

          <!-- PART 4: Binder mixer -->
          <rect x="315" y="130" width="80" height="80" rx="2" fill="#1e2220" stroke="#5d8f35" stroke-width="1.5"/>
          <!-- Mixer blade -->
          <circle cx="355" cy="170" r="25" fill="none" stroke="#3a403a" stroke-width="1"/>
          <line x1="355" y1="145" x2="355" y2="195" stroke="#7ab648" stroke-width="2.5"/>
          <line x1="330" y1="170" x2="380" y2="170" stroke="#7ab648" stroke-width="2.5"/>
          <line x1="338" y1="152" x2="372" y2="188" stroke="#5d8f35" stroke-width="1.5"/>
          <line x1="338" y1="188" x2="372" y2="152" stroke="#5d8f35" stroke-width="1.5"/>
          <!-- Spray nozzles -->
          <circle cx="318" cy="135" r="3" fill="#9fd063"/>
          <circle cx="392" cy="135" r="3" fill="#9fd063"/>
          <path d="M 318,138 L 325,150" stroke="#9fd063" stroke-width="1" opacity="0.6"/>
          <path d="M 392,138 L 385,150" stroke="#9fd063" stroke-width="1" opacity="0.6"/>
          <text x="355" y="225" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">MEZCLADOR</text>

          <!-- PART 5: Hydraulic piston -->
          <rect x="410" y="110" width="40" height="110" rx="2" fill="#242824" stroke="#8a9b8a" stroke-width="1.5"/>
          <rect x="418" y="120" width="24" height="50" rx="1" fill="#1e2220" stroke="#4d564d" stroke-width="1"/>
          <rect x="420" y="150" width="20" height="40" rx="1" fill="#2d322d" stroke="#5d8f35" stroke-width="2"/>
          <text x="430" y="235" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">PISTÓN</text>

          <!-- PART 6: Compaction chamber -->
          <rect x="455" y="140" width="90" height="60" rx="2" fill="#1e2220" stroke="#7ab648" stroke-width="2"/>
          <!-- Inner pressure lines -->
          <line x1="460" y1="155" x2="540" y2="155" stroke="#3a403a" stroke-width="0.5"/>
          <line x1="460" y1="165" x2="540" y2="165" stroke="#3a403a" stroke-width="0.5"/>
          <line x1="460" y1="175" x2="540" y2="175" stroke="#3a403a" stroke-width="0.5"/>
          <line x1="460" y1="185" x2="540" y2="185" stroke="#3a403a" stroke-width="0.5"/>
          <!-- Pressure arrows -->
          <path d="M 465,160 L 480,160 L 477,156 M 480,160 L 477,164" stroke="#7ab648" stroke-width="1.5" fill="none"/>
          <path d="M 535,170 L 520,170 L 523,166 M 520,170 L 523,174" stroke="#5d8f35" stroke-width="1.5" fill="none"/>
          <text x="500" y="215" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">CÁMARA COMPACTACIÓN</text>

          <!-- PART 7: Eccentric cam + flywheel -->
          <circle cx="630" cy="170" r="55" fill="#1e2220" stroke="#4d564d" stroke-width="1.5"/>
          <circle cx="630" cy="170" r="42" fill="none" stroke="#3a403a" stroke-width="1"/>
          <circle cx="630" cy="170" r="28" fill="#242824" stroke="#5d8f35" stroke-width="2"/>
          <circle cx="630" cy="170" r="8" fill="#2d322d" stroke="#7ab648" stroke-width="1.5"/>
          <!-- Flywheel spokes -->
          <line x1="630" y1="145" x2="630" y2="115" stroke="#4d564d" stroke-width="2.5"/>
          <line x1="630" y1="195" x2="630" y2="225" stroke="#4d564d" stroke-width="2.5"/>
          <line x1="605" y1="170" x2="575" y2="170" stroke="#4d564d" stroke-width="2.5"/>
          <line x1="655" y1="170" x2="685" y2="170" stroke="#4d564d" stroke-width="2.5"/>
          <line x1="611" y1="151" x2="591" y2="131" stroke="#3a403a" stroke-width="2"/>
          <line x1="649" y1="151" x2="669" y2="131" stroke="#3a403a" stroke-width="2"/>
          <!-- Eccentric cam offset circle -->
          <circle cx="645" cy="158" r="10" fill="#2d322d" stroke="#d4883c" stroke-width="1.5"/>
          <text x="630" y="240" fill="#6d7d6d" font-family="Barlow Condensed" font-size="9" text-anchor="middle">VOLANTE / LEVA EXCÉNTRICA</text>

          <!-- Connecting rod (piston to flywheel) -->
          <line x1="450" y1="170" x2="635" y2="170" stroke="#3a403a" stroke-width="3" stroke-dasharray="6,3"/>
          <!-- Arrow showing direction -->
          <path d="M 545,165 L 555,170 L 545,175" fill="#3a403a"/>

          <!-- PART 8: Output / briquette string -->
          <rect x="545" y="185" width="130" height="30" rx="3" fill="none" stroke="#3a403a" stroke-width="1" stroke-dasharray="3,3"/>
          <!-- Briquettes coming out -->
          <rect x="550" y="252" width="18" height="22" rx="9" fill="#8b5e3c" stroke="#c47a28" stroke-width="1"/>
          <rect x="572" y="252" width="18" height="22" rx="9" fill="#7d5434" stroke="#b56d20" stroke-width="1"/>
          <rect x="594" y="252" width="18" height="22" rx="9" fill="#8b5e3c" stroke="#c47a28" stroke-width="1"/>
          <rect x="616" y="252" width="18" height="22" rx="9" fill="#7d5434" stroke="#b56d20" stroke-width="1"/>
          <rect x="638" y="252" width="18" height="22" rx="9" fill="#8b5e3c" stroke="#c47a28" stroke-width="1"/>
          <!-- EcoBriq labels on briquettes -->
          <text x="559" y="265" fill="#c47a28" font-family="Barlow Condensed" font-size="6" text-anchor="middle" transform="rotate(-90,559,263)">ECO</text>

          <!-- PART 9: Cooling line (bottom) -->
          <rect x="30" y="290" width="510" height="14" rx="2" fill="#1a1e1a" stroke="#3a403a" stroke-width="1"/>
          <!-- Cooling fins -->
          <line x1="80" y1="290" x2="80" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="120" y1="290" x2="120" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="160" y1="290" x2="160" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="200" y1="290" x2="200" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="240" y1="290" x2="240" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="280" y1="290" x2="280" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="320" y1="290" x2="320" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="360" y1="290" x2="360" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="400" y1="290" x2="400" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="440" y1="290" x2="440" y2="304" stroke="#4d564d" stroke-width="1"/>
          <line x1="480" y1="290" x2="480" y2="304" stroke="#4d564d" stroke-width="1"/>
          <text x="265" y="325" fill="#3a403a" font-family="Barlow Condensed" font-size="9" text-anchor="middle">LÍNEA DE ENFRIAMIENTO</text>

          <!-- Dimension annotations -->
          <line x1="30" y1="360" x2="730" y2="360" stroke="#2a2e2a" stroke-width="0.5"/>
          <text x="380" y="375" fill="#3a403a" font-family="Barlow Condensed" font-size="8" text-anchor="middle">FLUJO DE MATERIAL: ASERRÍN → TRONCOS ECOLÓGICOS</text>
          
          <!-- Flow arrows along bottom -->
          <path d="M 80,350 L 90,355 L 80,360 M 90,355 L 650,355" stroke="#2d322d" stroke-width="1.5" fill="none"/>
          <path d="M 650,355 L 660,350 L 665,355 L 660,360 Z" fill="#2d322d"/>

          <!-- Motor symbol bottom right -->
          <rect x="680" y="268" width="50" height="40" rx="2" fill="#242824" stroke="#4d564d" stroke-width="1"/>
          <circle cx="705" cy="288" r="12" fill="#1e2220" stroke="#5d8f35" stroke-width="1.5"/>
          <text x="705" y="292" fill="#7ab648" font-family="Barlow Condensed" font-size="9" font-weight="700" text-anchor="middle">M</text>
          <text x="705" y="318" fill="#3a403a" font-family="Barlow Condensed" font-size="8" text-anchor="middle">MOTOR</text>

          <!-- Suction pipe (part connecting sawdust collection) -->
          <path d="M 60,80 Q 40,100 35,150 Q 33,200 35,290" stroke="#4d564d" stroke-width="2" fill="none" stroke-dasharray="4,2"/>

        </svg>

        <!-- Hotspot numbers (positioned over SVG) -->
        <!-- 1: Hopper/Feeding chute -->
        <div class="hotspot" id="h1" style="left:13.2%; top:16%" onclick="selectPart(1)">1</div>
        <!-- 2: Auger/Screw -->
        <div class="hotspot" id="h2" style="left:22%; top:47%" onclick="selectPart(2)">2</div>
        <!-- 3: Drying chamber -->
        <div class="hotspot" id="h3" style="left:36.8%; top:43%" onclick="selectPart(3)">3</div>
        <!-- 4: Binder mixer -->
        <div class="hotspot" id="h4" style="left:47.8%; top:43%" onclick="selectPart(4)">4</div>
        <!-- 5: Hydraulic piston -->
        <div class="hotspot" id="h5" style="left:57.5%; top:37%" onclick="selectPart(5)">5</div>
        <!-- 6: Compaction chamber -->
        <div class="hotspot" id="h6" style="left:66.7%; top:50%" onclick="selectPart(6)">6</div>
        <!-- 7: Flywheel / eccentric cam -->
        <div class="hotspot" id="h7" style="left:83.5%; top:43%" onclick="selectPart(7)">7</div>
        <!-- 8: Output briquettes -->
        <div class="hotspot" id="h8" style="left:78.5%; top:70%" onclick="selectPart(8)">8</div>
        <!-- 9: Cooling line -->
        <div class="hotspot" id="h9" style="left:36%; top:80%" onclick="selectPart(9)">9</div>

      </div>

      <!-- Process steps bar -->
      <div class="process-bar" id="processBar">
        <div class="process-step" onclick="selectPart(1)" id="s1">
          <span class="step-num">1</span>
          <span class="step-label">Recolección</span>
        </div>
        <div class="process-step" onclick="selectPart(2)" id="s2">
          <span class="step-num">2</span>
          <span class="step-label">Transporte</span>
        </div>
        <div class="process-step" onclick="selectPart(3)" id="s3">
          <span class="step-num">3</span>
          <span class="step-label">Secado</span>
        </div>
        <div class="process-step" onclick="selectPart(4)" id="s4">
          <span class="step-num">4</span>
          <span class="step-label">Mezcla</span>
        </div>
        <div class="process-step" onclick="selectPart(5)" id="s5">
          <span class="step-num">5</span>
          <span class="step-label">Compresión</span>
        </div>
        <div class="process-step" onclick="selectPart(6)" id="s6">
          <span class="step-num">6</span>
          <span class="step-label">Formación</span>
        </div>
        <div class="process-step" onclick="selectPart(7)" id="s7">
          <span class="step-num">7</span>
          <span class="step-label">Transmisión</span>
        </div>
        <div class="process-step" onclick="selectPart(8)" id="s8">
          <span class="step-num">8</span>
          <span class="step-label">Salida</span>
        </div>
        <div class="process-step" onclick="selectPart(9)" id="s9">
          <span class="step-num">9</span>
          <span class="step-label">Enfriamiento</span>
        </div>
      </div>

    </div>
  </div>

  <!-- RIGHT PANEL -->
  <div class="info-panel">

    <div id="infoDisplay">
      <div class="info-body">
        <div class="info-placeholder">
          <div class="placeholder-icon">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#3a403a" stroke-width="1.5">
              <circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/>
            </svg>
          </div>
          <div class="placeholder-text">
            Selecciona un componente en el diagrama o en la barra de proceso para ver su descripción detallada, composición y función dentro del sistema EcoBriq.
          </div>
        </div>
      </div>
    </div>

    <div class="metrics-row">
      <div class="metric-card">
        <span class="metric-val">9</span>
        <span class="metric-label">Etapas proceso</span>
      </div>
      <div class="metric-card">
        <span class="metric-val">&lt;15%</span>
        <span class="metric-label">Humedad final</span>
      </div>
      <div class="metric-card">
        <span class="metric-val">B2B</span>
        <span class="metric-label">Distribución</span>
      </div>
    </div>

  </div>

</div>

<script>
const parts = {
  1: {
    num: "01",
    name: "Tolva de alimentación",
    subtitle: "Punto de ingreso del material",
    desc: "La tolva es el componente de entrada del sistema. Recibe el aserrín generado por el proceso de aserrado y lo canaliza de forma controlada hacia el tornillo sin fin. Su geometría trapezoidal asegura un flujo gravitacional continuo sin atascos.",
    specs: [
      { k: "Material", v: "Acero inoxidable 304" },
      { k: "Ángulo de inclinación", v: "45–60°" },
      { k: "Capacidad aprox.", v: "50–80 kg" },
      { k: "Conexión", v: "Brida soldada al bastidor" }
    ],
    materials: ["Acero inox.", "Soldadura MIG", "Brida de fijación"],
    color: "#5d8f35"
  },
  2: {
    num: "02",
    name: "Tornillo sin fin",
    subtitle: "Transporte automatizado del aserrín",
    desc: "El tornillo sin fin (auger) es el mecanismo de transporte que desplaza el aserrín desde la tolva hacia las etapas de proceso. Elimina completamente el traslado manual, reduce los tiempos muertos y garantiza un flujo constante y uniforme del material.",
    specs: [
      { k: "Tipo", v: "Helicoidal / Arquimediano" },
      { k: "Material", v: "Acero al carbono" },
      { k: "Diámetro del tubo", v: "150 mm" },
      { k: "Velocidad", v: "Regulable por variador" }
    ],
    materials: ["Acero al carbono", "Chumaceras", "Sellado con teflon", "Motor reductor"],
    color: "#7ab648"
  },
  3: {
    num: "03",
    name: "Cámara de secado",
    subtitle: "Reducción de humedad del material",
    desc: "La cámara de secado reduce la humedad del aserrín hasta valores inferiores al 15%, condición crítica para lograr una buena compactación. Utiliza el calor residual generado por los motores del propio aserradero, aprovechando energía que de otro modo se desperdiciaría.",
    specs: [
      { k: "Fuente de calor", v: "Calor residual motores" },
      { k: "Temperatura operación", v: "60–90 °C" },
      { k: "Humedad objetivo", v: "< 15%" },
      { k: "Tiempo de residencia", v: "Variable según material" }
    ],
    materials: ["Carcasa acero galvanizado", "Aislante térmico", "Sensores de humedad", "Control PID"],
    color: "#d4883c"
  },
  4: {
    num: "04",
    name: "Mezclador con aglutinante",
    subtitle: "Incorporación del agente ligante",
    desc: "El mezclador incorpora un aglutinante natural —almidón de yuca o lignina— al aserrín seco mediante aspersores. Esta mezcla homogénea es fundamental para lograr troncos de alta densidad y cohesión uniforme durante la compactación. El uso de aglutinantes naturales garantiza que el producto final sea 100% ecológico y libre de sustancias químicas.",
    specs: [
      { k: "Aglutinante", v: "Almidón yuca / Lignina" },
      { k: "Incorporación", v: "Aspersores dosificadores" },
      { k: "Tipo mezclado", v: "Paletas helicoidales" },
      { k: "Control", v: "Dosificación proporcional" }
    ],
    materials: ["Paletas de acero inox.", "Bomba dosificadora", "Aspersores de nebulización", "Sensores caudal"],
    color: "#9fd063"
  },
  5: {
    num: "05",
    name: "Pistón hidráulico",
    subtitle: "Mecanismo de compresión a alta presión",
    desc: "El pistón hidráulico aplica la fuerza de compresión sobre la mezcla de aserrín y aglutinante dentro de la cámara de compactación. Es el elemento activo que transforma el material suelto en troncos de alta densidad. El movimiento alternativo del pistón es generado por la leva excéntrica del volante.",
    specs: [
      { k: "Tipo", v: "Pistón de simple efecto" },
      { k: "Presión de trabajo", v: "Alta presión" },
      { k: "Accionamiento", v: "Mecánico / leva excéntrica" },
      { k: "Material camisa", v: "Acero templado" }
    ],
    materials: ["Acero templado", "Sellos hidráulicos", "Guías de bronce", "Lubricación centralizada"],
    color: "#8a9b8a"
  },
  6: {
    num: "06",
    name: "Cámara de compactación",
    subtitle: "Formación del tronco ecológico",
    desc: "En la cámara de compactación ocurre la transformación central del proceso: la mezcla de aserrín con aglutinante se comprime a alta presión para formar troncos cilíndricos de alta densidad y estructura homogénea. La forma cilíndrica se obtiene por la geometría de la cámara y el molde de salida.",
    specs: [
      { k: "Forma del producto", v: "Cilíndrica" },
      { k: "Densidad objetivo", v: "Alta densidad uniforme" },
      { k: "Material cámara", v: "Acero endurecido" },
      { k: "Salida", v: "Continua por extrusión" }
    ],
    materials: ["Acero endurecido HRC50+", "Molde de extrusión", "Revestimiento antidesgaste"],
    color: "#7ab648"
  },
  7: {
    num: "07",
    name: "Volante y leva excéntrica",
    subtitle: "Sistema de transmisión de potencia",
    desc: "El volante de inercia almacena energía cinética y regula la uniformidad del movimiento del sistema. La leva excéntrica convierte el movimiento rotatorio del motor en el movimiento lineal alternativo del pistón. Juntos forman el corazón mecánico que impulsa todo el proceso de compactación.",
    specs: [
      { k: "Función volante", v: "Almacenamiento de inercia" },
      { k: "Función leva", v: "Conversión rot. → lineal" },
      { k: "Material volante", v: "Hierro fundido" },
      { k: "Conexión", v: "Eje motor + biela" }
    ],
    materials: ["Hierro fundido gris", "Rodamientos de bolas", "Biela de acero", "Leva de acero templado"],
    color: "#d4883c"
  },
  8: {
    num: "08",
    name: "Salida de troncos (EcoBriq)",
    subtitle: "Producto final listo para distribución",
    desc: "En la zona de salida, los troncos ecológicos emergen de forma continua con su forma cilíndrica definitiva. Aquí se produce el corte a la longitud deseada y los troncos se apilan para su posterior enfriamiento y empaque. Cada tronco EcoBriq es apto para uso en estufas a leña, calderas y cocinas de combustión lenta.",
    specs: [
      { k: "Destino", v: "Estufas, calderas, chimeneas" },
      { k: "Mercado", v: "B2B: industria y agroindustria" },
      { k: "Contenido humedad", v: "< 15%" },
      { k: "Corte", v: "Longitud regulable" }
    ],
    materials: ["Aserrín compactado", "Aglutinante natural", "Sin aditivos químicos"],
    color: "#c47a28"
  },
  9: {
    num: "09",
    name: "Línea de enfriamiento",
    subtitle: "Estabilización y almacenamiento del producto",
    desc: "Tras la compactación, los troncos pasan por la línea de enfriamiento donde se estabilizan estructuralmente. El enfriamiento progresivo permite que el aglutinante fragüe correctamente y que los troncos adquieran su resistencia final antes de ser apilados, empacados y distribuidos.",
    specs: [
      { k: "Sistema", v: "Convección natural / forzada" },
      { k: "Longitud línea", v: "Según producción" },
      { k: "Temperatura salida", v: "Ambiente" },
      { k: "Posterior paso", v: "Empaque y distribución" }
    ],
    materials: ["Estructura acero", "Rodillos de transporte", "Ventiladores (opcional)", "Zona de apilado"],
    color: "#4d564d"
  }
};

function selectPart(num) {
  // Reset all
  document.querySelectorAll('.hotspot').forEach(h => h.classList.remove('active'));
  document.querySelectorAll('.process-step').forEach(s => s.classList.remove('active'));

  // Activate selected
  document.getElementById('h' + num).classList.add('active');
  document.getElementById('s' + num).classList.add('active');

  const p = parts[num];
  const accentColor = p.color;

  const specsHtml = p.specs.map(s => `
    <div class="spec-row">
      <span class="spec-key">${s.k}</span>
      <span class="spec-val">${s.v}</span>
    </div>
  `).join('');

  const materialsHtml = p.materials.map(m => `<span class="material-tag">${m}</span>`).join('');

  document.getElementById('infoDisplay').innerHTML = `
    <div class="info-header">
      <div class="info-part-num">${p.num}</div>
      <div class="info-part-name" style="color:${accentColor}">${p.name}</div>
      <div class="info-part-subtitle">${p.subtitle}</div>
    </div>
    <div class="info-body">
      <div class="info-section">
        <div class="info-section-label">Función en el sistema</div>
        <div class="info-desc">${p.desc}</div>
      </div>
      <div class="info-section">
        <div class="info-section-label">Especificaciones técnicas</div>
        <div class="info-specs">${specsHtml}</div>
      </div>
      <div class="info-section">
        <div class="info-section-label">Materiales y componentes</div>
        <div>${materialsHtml}</div>
      </div>
    </div>
  `;
}
</script>

</body>
</html>
