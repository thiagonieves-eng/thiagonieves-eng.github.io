<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Thiago Mathias Nieves Checca</title>
  <meta name="description" content="Thiago Mathias Nieves Checca — Estudiante de Ciencias de la Computación en la Universidad Católica San Pablo, Arequipa, Perú."/>
  <meta name="author" content="Thiago Mathias Nieves Checca"/>
  <meta name="keywords" content="Thiago Nieves, Thiago Mathias Nieves Checca, UCSP, Ciencias de la Computación, Arequipa, Peru, estudiante programacion"/>
  <meta property="og:title" content="Thiago Mathias Nieves Checca"/>
  <meta property="og:description" content="Thiago Mathias Nieves Checca — Estudiante de Ciencias de la Computación en la UCSP, Arequipa."/>
  <meta property="og:type" content="website"/>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --bg: #0a0f1a;
      --surface: #111827;
      --border: #1e2d42;
      --accent: #3b82f6;
      --accent2: #60a5fa;
      --green: #22c55e;
      --text: #e2e8f0;
      --muted: #64748b;
      --tag-bg: #1e2d42;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'Space Grotesk', sans-serif;
      line-height: 1.6;
      min-height: 100vh;
    }

    nav {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(10, 15, 26, 0.92);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
      padding: 0 40px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 60px;
    }

    .nav-logo {
      font-family: 'Space Mono', monospace;
      font-size: 14px;
      color: var(--accent2);
      letter-spacing: 1px;
    }

    .nav-links {
      display: flex;
      gap: 32px;
      list-style: none;
    }

    .nav-links a {
      font-size: 13px;
      color: var(--muted);
      text-decoration: none;
      transition: color 0.2s;
    }

    .nav-links a:hover { color: var(--text); }

    .hero {
      max-width: 860px;
      margin: 0 auto;
      padding: 100px 40px 80px;
    }

    .hero-eyebrow {
      font-family: 'Space Mono', monospace;
      font-size: 11px;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .hero-eyebrow::before {
      content: '';
      width: 24px;
      height: 1px;
      background: var(--accent);
    }

    .hero h1 {
      font-size: clamp(36px, 6vw, 64px);
      font-weight: 700;
      line-height: 1.05;
      letter-spacing: -1px;
      margin-bottom: 24px;
    }

    .hero h1 span { color: var(--accent2); }

    .hero-desc {
      font-size: 17px;
      color: var(--muted);
      max-width: 560px;
      line-height: 1.8;
      margin-bottom: 40px;
    }

    .hero-badges {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 40px;
    }

    .badge {
      background: var(--tag-bg);
      border: 1px solid var(--border);
      color: var(--accent2);
      font-size: 12px;
      font-family: 'Space Mono', monospace;
      padding: 6px 14px;
      border-radius: 4px;
    }

    .hero-links {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 12px 24px;
      border-radius: 6px;
      font-size: 14px;
      font-weight: 600;
      text-decoration: none;
      transition: all 0.2s;
    }

    .btn-primary { background: var(--accent); color: #fff; }
    .btn-primary:hover { background: #2563eb; transform: translateY(-1px); }

    .btn-secondary {
      background: transparent;
      color: var(--text);
      border: 1px solid var(--border);
    }
    .btn-secondary:hover { border-color: var(--accent2); color: var(--accent2); transform: translateY(-1px); }

    .section {
      max-width: 860px;
      margin: 0 auto;
      padding: 60px 40px;
      border-top: 1px solid var(--border);
    }

    .section-label {
      font-family: 'Space Mono', monospace;
      font-size: 10px;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 8px;
    }

    .section-title {
      font-size: 28px;
      font-weight: 700;
      letter-spacing: -0.5px;
      margin-bottom: 32px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
      gap: 16px;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 20px;
      text-decoration: none;
      color: var(--text);
      transition: all 0.2s;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .card:hover {
      border-color: var(--accent);
      transform: translateY(-2px);
      box-shadow: 0 8px 24px rgba(59, 130, 246, 0.08);
    }

    .card-course {
      font-size: 11px;
      font-family: 'Space Mono', monospace;
      color: var(--accent2);
      letter-spacing: 0.5px;
    }

    .card-name { font-size: 15px; font-weight: 600; }
    .card-sub { font-size: 12px; color: var(--muted); }
    .card-link-label { font-size: 11px; color: var(--accent); margin-top: 4px; }
    .card-link-label.email { color: var(--green); }

    .comp-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
      gap: 12px;
    }

    .comp-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 20px 16px;
      text-decoration: none;
      color: var(--text);
      text-align: center;
      transition: all 0.2s;
    }

    .comp-card:hover {
      border-color: var(--green);
      transform: translateY(-2px);
      box-shadow: 0 8px 24px rgba(34, 197, 94, 0.08);
    }

    .comp-avatar {
      width: 48px;
      height: 48px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--accent), var(--green));
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 700;
      font-size: 18px;
      margin: 0 auto 12px;
      color: #fff;
    }

    .comp-name { font-size: 14px; font-weight: 600; }
    .comp-link { font-size: 11px; color: var(--green); margin-top: 4px; font-family: 'Space Mono', monospace; }

    footer {
      text-align: center;
      padding: 40px;
      border-top: 1px solid var(--border);
      font-size: 12px;
      color: var(--muted);
      font-family: 'Space Mono', monospace;
    }

    .fade-in { opacity: 0; transform: translateY(20px); transition: opacity 0.5s ease, transform 0.5s ease; }
    .fade-in.visible { opacity: 1; transform: translateY(0); }

    @media (max-width: 600px) {
      nav { padding: 0 20px; }
      .hero, .section { padding-left: 20px; padding-right: 20px; }
      .nav-links { display: none; }
    }
  </style>
</head>
<body>

<nav>
  <div class="nav-logo">Thiago Mathias Nieves Checca</div>
  <ul class="nav-links">
    <li><a href="#sobre-mi">Sobre mí</a></li>
    <li><a href="#profesores">Profesores</a></li>
    <li><a href="#companeros">Compañeros</a></li>
  </ul>
</nav>

<section class="hero" id="sobre-mi">
  <div class="hero-eyebrow">Ciencias de la Computación — UCSP</div>
  <h1>Hola, soy<br><span>Thiago Mathias</span><br>Nieves Checca</h1>
  <p class="hero-desc">
    Tengo 17 años y estoy cursando el primer semestre de Ciencias de la Computación en la Universidad Católica San Pablo de Arequipa. Me apasiona aprender, resolver problemas y trabajar en equipo. Fuera de las aulas, el deporte es parte esencial de mi día a día.
  </p>
  <div class="hero-badges">
    <span class="badge">Trabajo en equipo</span>
    <span class="badge">Proactividad</span>
    <span class="badge">Responsabilidad</span>
    <span class="badge">Pensamiento analítico</span>
    <span class="badge">Deporte &amp; disciplina</span>
    <span class="badge">Aprendizaje continuo</span>
  </div>
  <div class="hero-links">
    <a class="btn btn-primary" href="https://www.linkedin.com/in/thiago-mathias-nieves-checca-34b606411" target="_blank" rel="noopener">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      LinkedIn
    </a>
    <a class="btn btn-secondary" href="https://github.com/thiagonieves-eng" target="_blank" rel="noopener">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
      GitHub
    </a>
  </div>
</section>

<section class="section fade-in" id="profesores">
  <div class="section-label">Primer semestre 2025</div>
  <h2 class="section-title">Mis profesores</h2>
  <div class="grid">

    <a class="card" href="mailto:sgsuarez@ucsp.edu.pe">
      <div class="card-course">Fundamentos Matemáticos</div>
      <div class="card-name">Sabrina Suárez</div>
      <div class="card-sub">Fundamentos matemáticos para la computación</div>
      <div class="card-link-label email">✉ sgsuarez@ucsp.edu.pe</div>
    </a>

    <a class="card" href="https://pe.linkedin.com/in/kelly-vizconde-la-motta-3a57a4143" target="_blank" rel="noopener">
      <div class="card-course">Fundamentos de Programación</div>
      <div class="card-name">Kelly Vizconde La Motta</div>
      <div class="card-sub">Fundamentos de programación</div>
      <div class="card-link-label">↗ Ver LinkedIn</div>
    </a>

    <a class="card" href="https://pe.linkedin.com/in/angel-rodriguez-cruz-58b78b85" target="_blank" rel="noopener">
      <div class="card-course">Comunicación</div>
      <div class="card-name">Ángel Rodríguez Cruz</div>
      <div class="card-sub">Comunicación</div>
      <div class="card-link-label">↗ Ver LinkedIn</div>
    </a>

    <a class="card" href="https://pe.linkedin.com/in/yahaira-byrne-rivera-274201221" target="_blank" rel="noopener">
      <div class="card-course">Lógica</div>
      <div class="card-name">Yahaira Byrne Rivera</div>
      <div class="card-sub">Lógica</div>
      <div class="card-link-label">↗ Ver LinkedIn</div>
    </a>

    <a class="card" href="https://pe.linkedin.com/in/ecuadrosv" target="_blank" rel="noopener">
      <div class="card-course">Fundamentos de Computación</div>
      <div class="card-name">Ernesto Cuadros</div>
      <div class="card-sub">Fundamentos de computación</div>
      <div class="card-link-label">↗ Ver LinkedIn</div>
    </a>

    <a class="card" href="mailto:pierina.pacheco@ucsp.edu.pe">
      <div class="card-course">Vida Universitaria</div>
      <div class="card-name">Pierina Pacheco Leyton</div>
      <div class="card-sub">Introducción a la vida universitaria</div>
      <div class="card-link-label email">✉ pierina.pacheco@ucsp.edu.pe</div>
    </a>

  </div>
</section>

<section class="section fade-in" id="companeros">
  <div class="section-label">Ciencias de la Computación — UCSP</div>
  <h2 class="section-title">Mis compañeros</h2>
  <div class="comp-grid">

    <a class="comp-card" href="https://ackyul.github.io" target="_blank" rel="noopener">
      <div class="comp-avatar">Y</div>
      <div class="comp-name">Yohsua</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

    <a class="comp-card" href="https://vargaslazo.github.io/" target="_blank" rel="noopener">
      <div class="comp-avatar">J</div>
      <div class="comp-name">Josué</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

    <a class="comp-card" href="https://michaelerickconchayucra.github.io/" target="_blank" rel="noopener">
      <div class="comp-avatar">E</div>
      <div class="comp-name">Eric</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

    <a class="comp-card" href="https://bryanalencastre.github.io/Bryan-Alencastre/" target="_blank" rel="noopener">
      <div class="comp-avatar">G</div>
      <div class="comp-name">Gabriel</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

    <a class="comp-card" href="https://yulvillena-source.github.io/Yul_Villena/" target="_blank" rel="noopener">
      <div class="comp-avatar">Y</div>
      <div class="comp-name">Yul</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

    <a class="comp-card" href="https://angelfabianramosmunoz.github.io/" target="_blank" rel="noopener">
      <div class="comp-avatar">A</div>
      <div class="comp-name">Angel</div>
      <div class="comp-link">↗ Ver página</div>
    </a>

  </div>
</section>

<footer>
  <p>Thiago Mathias Nieves Checca &nbsp;·&nbsp; UCSP Arequipa &nbsp;·&nbsp; 2025</p>
</footer>

<script>
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) e.target.classList.add('visible');
    });
  }, { threshold: 0.1 });
  document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
</script>

</body>
</html>
