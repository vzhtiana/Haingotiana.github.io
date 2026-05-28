# Haingotiana.github.io
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Zo Haingotiana VOLOLONJANAHARY | Portfolio</title>
  <meta name="description" content="Portfolio professionnel de Zo Haingotiana VOLOLONJANAHARY, System & Network Administrator basé à Antsirabe, Madagascar." />
  <style>
    :root {
      --bg: #0b1020;
      --bg-soft: #121933;
      --card: rgba(255,255,255,0.06);
      --card-border: rgba(255,255,255,0.10);
      --text: #eef2ff;
      --muted: #b8c0e0;
      --primary: #6ea8fe;
      --secondary: #73e0c2;
      --accent: #8b7cff;
      --shadow: 0 20px 60px rgba(0,0,0,0.35);
      --radius: 22px;
      --max: 1180px;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
      color: var(--text);
      background:
        radial-gradient(circle at top left, rgba(110,168,254,0.20), transparent 28%),
        radial-gradient(circle at top right, rgba(115,224,194,0.18), transparent 22%),
        radial-gradient(circle at 50% 100%, rgba(139,124,255,0.14), transparent 30%),
        linear-gradient(180deg, #09101f 0%, #0b1020 100%);
      line-height: 1.65;
    }

    a { color: inherit; text-decoration: none; }
    img { max-width: 100%; display: block; }

    .container {
      width: min(var(--max), calc(100% - 32px));
      margin: 0 auto;
    }

    .nav {
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(14px);
      background: rgba(7, 11, 24, 0.68);
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }

    .nav-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 16px 0;
      gap: 18px;
    }

    .brand {
      display: flex;
      flex-direction: column;
      gap: 2px;
    }

    .brand strong {
      font-size: 0.98rem;
      letter-spacing: 0.02em;
    }

    .brand span {
      color: var(--muted);
      font-size: 0.88rem;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      justify-content: flex-end;
    }

    .nav-links a {
      color: var(--muted);
      font-size: 0.95rem;
      transition: 0.2s ease;
    }

    .nav-links a:hover { color: var(--text); }

    .hero {
      padding: 80px 0 42px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.35fr 0.95fr;
      gap: 26px;
      align-items: stretch;
    }

    .hero-card, .panel {
      background: var(--card);
      border: 1px solid var(--card-border);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }

    .hero-card {
      padding: 34px;
      position: relative;
      overflow: hidden;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 14px;
      border-radius: 999px;
      background: rgba(110,168,254,0.14);
      color: #dce8ff;
      border: 1px solid rgba(110,168,254,0.22);
      font-size: 0.9rem;
      margin-bottom: 18px;
    }

    h1, h2, h3 { margin: 0 0 14px; line-height: 1.14; }
    h1 {
      font-size: clamp(2.35rem, 5vw, 4.4rem);
      letter-spacing: -0.04em;
      max-width: 12ch;
    }

    .lead {
      font-size: 1.06rem;
      color: var(--muted);
      max-width: 62ch;
      margin-bottom: 24px;
    }

    .hero-actions {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
      margin-bottom: 28px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 14px 18px;
      border-radius: 14px;
      font-weight: 600;
      transition: transform 0.2s ease, background 0.2s ease, border-color 0.2s ease;
      border: 1px solid transparent;
    }

    .btn:hover { transform: translateY(-2px); }
    .btn-primary {
      background: linear-gradient(135deg, var(--primary), var(--accent));
      color: white;
    }

    .btn-secondary {
      background: rgba(255,255,255,0.04);
      border-color: rgba(255,255,255,0.12);
      color: var(--text);
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(3, minmax(0,1fr));
      gap: 14px;
    }

    .stat {
      padding: 18px;
      border-radius: 18px;
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.08);
    }

    .stat strong {
      display: block;
      font-size: 1.4rem;
      margin-bottom: 6px;
    }

    .stat span {
      color: var(--muted);
      font-size: 0.92rem;
    }

    .profile {
      padding: 26px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      gap: 22px;
    }

    .avatar {
      width: 78px;
      height: 78px;
      border-radius: 22px;
      display: grid;
      place-items: center;
      font-size: 1.5rem;
      font-weight: 800;
      background: linear-gradient(135deg, rgba(110,168,254,0.24), rgba(115,224,194,0.2));
      border: 1px solid rgba(255,255,255,0.14);
    }

    .mini-title {
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 0.75rem;
      margin-bottom: 8px;
    }

    .profile h2 { font-size: 1.6rem; }

    .contact-list {
      display: grid;
      gap: 12px;
    }

    .contact-item {
      padding: 14px 16px;
      border-radius: 16px;
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.08);
    }

    .contact-item small {
      display: block;
      color: var(--muted);
      margin-bottom: 4px;
    }

    section {
      padding: 24px 0;
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: end;
      gap: 16px;
      margin-bottom: 18px;
    }

    .section-header p {
      margin: 0;
      color: var(--muted);
      max-width: 64ch;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
    }

    .card {
      background: var(--card);
      border: 1px solid var(--card-border);
      border-radius: 20px;
      padding: 24px;
      box-shadow: var(--shadow);
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .chip {
      padding: 10px 12px;
      border-radius: 999px;
      font-size: 0.92rem;
      color: #e8edff;
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.08);
    }

    .projects {
      display: grid;
      grid-template-columns: repeat(2, minmax(0,1fr));
      gap: 20px;
    }

    .project {
      padding: 24px;
      border-radius: 22px;
      background: linear-gradient(180deg, rgba(255,255,255,0.065), rgba(255,255,255,0.04));
      border: 1px solid rgba(255,255,255,0.1);
      box-shadow: var(--shadow);
    }

    .project .tag {
      display: inline-block;
      margin-bottom: 12px;
      padding: 7px 12px;
      border-radius: 999px;
      font-size: 0.82rem;
      color: #dfe8ff;
      background: rgba(110,168,254,0.14);
      border: 1px solid rgba(110,168,254,0.22);
    }

    .project p { color: var(--muted); margin: 0 0 12px; }

    .project ul {
      padding-left: 18px;
      margin: 0;
      color: #dee6ff;
    }

    .timeline {
      display: grid;
      gap: 18px;
    }

    .timeline-item {
      position: relative;
      padding: 20px 20px 20px 24px;
      border-radius: 20px;
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.08);
      overflow: hidden;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      inset: 0 auto 0 0;
      width: 4px;
      background: linear-gradient(180deg, var(--primary), var(--secondary));
    }

    .timeline-top {
      display: flex;
      justify-content: space-between;
      gap: 16px;
      flex-wrap: wrap;
      margin-bottom: 10px;
    }

    .timeline-top span {
      color: var(--muted);
      font-size: 0.92rem;
    }

    .timeline p { margin: 0; color: var(--muted); }

    .education, .languages {
      display: grid;
      gap: 14px;
    }

    .edu-item, .lang-item {
      padding: 18px;
      border-radius: 18px;
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.08);
    }

    .cta {
      margin: 26px 0 70px;
      padding: 32px;
      border-radius: 26px;
      background: linear-gradient(135deg, rgba(110,168,254,0.16), rgba(115,224,194,0.12), rgba(139,124,255,0.12));
      border: 1px solid rgba(255,255,255,0.12);
      box-shadow: var(--shadow);
      display: flex;
      justify-content: space-between;
      gap: 20px;
      align-items: center;
      flex-wrap: wrap;
    }

    .cta p { margin: 0; color: var(--muted); max-width: 60ch; }

    footer {
      padding: 0 0 34px;
      color: var(--muted);
      font-size: 0.94rem;
    }

    @media (max-width: 980px) {
      .hero-grid, .grid-2, .projects { grid-template-columns: 1fr; }
      .stats { grid-template-columns: 1fr; }
      .nav-inner { align-items: flex-start; flex-direction: column; }
      .nav-links { justify-content: flex-start; }
    }

    @media (max-width: 640px) {
      .hero { padding-top: 56px; }
      .hero-card, .profile, .card, .project, .cta { padding: 22px; }
      .container { width: min(var(--max), calc(100% - 20px)); }
      h1 { max-width: none; }
    }
  </style>
</head>
<body>
  <header class="nav">
    <div class="container nav-inner">
      <div class="brand">
        <strong>Zo Haingotiana VOLOLONJANAHARY</strong>
        <span>System & Network Administrator</span>
      </div>
      <nav class="nav-links">
        <a href="#apropos">À propos</a>
        <a href="#competences">Compétences</a>
        <a href="#projets">Réalisations</a>
        <a href="#experience">Expérience</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-grid">
        <div class="hero-card">
          <div class="badge">Infrastructure • Sécurité • Continuité de service</div>
          <h1>Administrateur Système & Réseau</h1>
          <p class="lead">
            Je conçois, sécurise et maintiens des environnements IT fiables pour des organisations exigeantes. Mon expertise couvre les systèmes Windows/Linux, Microsoft 365, Azure, la virtualisation, les sauvegardes, le support utilisateurs et l’exploitation en contexte de production.
          </p>
          <div class="hero-actions">
            <a class="btn btn-primary" href="#contact">Me contacter</a>
            <a class="btn btn-secondary" href="#projets">Voir les réalisations</a>
          </div>
          <div class="stats">
            <div class="stat">
              <strong>99,8 %</strong>
              <span>de disponibilité atteinte sur une infrastructure en production</span>
            </div>
            <div class="stat">
              <strong>80</strong>
              <span>utilisateurs accompagnés dans un environnement opérationnel</span>
            </div>
            <div class="stat">
              <strong>5+ ans</strong>
              <span>d’expérience en administration systèmes & réseaux</span>
            </div>
          </div>
        </div>

        <aside class="panel profile" id="contact">
          <div>
            <div class="avatar">ZH</div>
          </div>
          <div>
            <div class="mini-title">Profil</div>
            <h2>Zo Haingotiana VOLOLONJANAHARY</h2>
            <p style="color: var(--muted); margin-top: 0;">
              Basé à Antsirabe, Madagascar, j’interviens sur des environnements de production avec une approche pragmatique, orientée résultats, sécurité et stabilité.
            </p>
          </div>
          <div class="contact-list">
            <div class="contact-item">
              <small>Email</small>
              <a href="mailto:zohtiana@gmail.com">zohtiana@gmail.com</a>
            </div>
            <div class="contact-item">
              <small>Téléphone</small>
              <a href="tel:+261341985702">+261 34 19 857 02</a>
            </div>
            <div class="contact-item">
              <small>Localisation</small>
              <span>Ambohimena, Antsirabe, Madagascar</span>
            </div>
            <div class="contact-item">
              <small>LinkedIn / Profil public</small>
              <span>Zo Haingotiana</span>
            </div>
          </div>
        </aside>
      </div>
    </section>

    <section id="apropos">
      <div class="container grid-2">
        <div class="card">
          <div class="mini-title">À propos</div>
          <h2>Un profil IT polyvalent, orienté fiabilité</h2>
          <p>
            Je suis spécialisé en administration systèmes et réseaux avec une forte expérience sur les environnements Microsoft, les serveurs Windows/Linux, la sécurité opérationnelle, la virtualisation et le support utilisateurs. J’ai évolué dans des contextes multi-sites, internationaux et hybrides où la continuité de service, la performance et la sécurisation sont essentielles.
          </p>
          <p>
            Mon parcours me permet de relier l’infrastructure, les besoins métier et les usages utilisateurs. En complément de mes compétences cœur en exploitation IT, j’ai aussi une expérience en ERP, scripting, développement applicatif et UI/UX, ce qui me donne une vision globale des systèmes d’information.
          </p>
        </div>
        <div class="card">
          <div class="mini-title">Ce qui me distingue</div>
          <h2>Valeur ajoutée</h2>
          <div class="chips">
            <span class="chip">Windows Server & Active Directory</span>
            <span class="chip">Linux & environnements hybrides</span>
            <span class="chip">Microsoft 365 & Azure</span>
            <span class="chip">VMware & Proxmox</span>
            <span class="chip">Veeam & continuité d’activité</span>
            <span class="chip">ISO 27001 & sécurité opérationnelle</span>
            <span class="chip">Support L1 / L2 / L3</span>
            <span class="chip">ERP, scripting & UI/UX</span>
          </div>
        </div>
      </div>
    </section>

    <section id="competences">
      <div class="container">
        <div class="section-header">
          <div>
            <div class="mini-title">Compétences</div>
            <h2>Expertises techniques</h2>
          </div>
          <p>
            Un socle technique construit autour de l’administration système, du cloud, de la sécurité, du support et des outils métiers.
          </p>
        </div>
        <div class="grid-2">
          <div class="card">
            <h3>Systèmes & infrastructure</h3>
            <div class="chips">
              <span class="chip">Windows Server 2008/2012/2016/2019</span>
              <span class="chip">Active Directory</span>
              <span class="chip">GPO</span>
              <span class="chip">Linux Debian / Ubuntu / CentOS</span>
              <span class="chip">macOS</span>
              <span class="chip">Microsoft 365</span>
              <span class="chip">SharePoint</span>
              <span class="chip">Exchange / mail local</span>
            </div>
          </div>
          <div class="card">
            <h3>Cloud, virtualisation & sauvegarde</h3>
            <div class="chips">
              <span class="chip">Azure</span>
              <span class="chip">VMware</span>
              <span class="chip">Proxmox</span>
              <span class="chip">Veeam Data Cloud</span>
              <span class="chip">Backup systems</span>
              <span class="chip">RBAC</span>
              <span class="chip">NSG</span>
              <span class="chip">VPN</span>
            </div>
          </div>
          <div class="card">
            <h3>Réseau & cybersécurité</h3>
            <div class="chips">
              <span class="chip">Cisco</span>
              <span class="chip">Sophos Firewall</span>
              <span class="chip">Ubiquiti</span>
              <span class="chip">FortiClient VPN</span>
              <span class="chip">VLAN</span>
              <span class="chip">MFA</span>
              <span class="chip">ISO 27001</span>
              <span class="chip">Monitoring</span>
            </div>
          </div>
          <div class="card">
            <h3>Développement, ERP & collaboration</h3>
            <div class="chips">
              <span class="chip">Python</span>
              <span class="chip">.NET / ASP.NET</span>
              <span class="chip">Java / Java EE</span>
              <span class="chip">SQL</span>
              <span class="chip">Odoo</span>
              <span class="chip">Sage 100</span>
              <span class="chip">Microsoft Navision</span>
              <span class="chip">Figma</span>
              <span class="chip">React Native</span>
              <span class="chip">Talend Studio</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="projets">
      <div class="container">
        <div class="section-header">
          <div>
            <div class="mini-title">Réalisations</div>
            <h2>Projets à fort impact</h2>
          </div>
          <p>
            Une sélection de missions qui illustrent ma capacité à sécuriser, stabiliser et faire évoluer des environnements IT réels.
          </p>
        </div>
        <div class="projects">
          <article class="project">
            <span class="tag">UCC EXPERTS France</span>
            <h3>Conformité ISO 27001 & sécurisation Azure</h3>
            <p>
              Mise en œuvre de procédures IT conformes ISO 27001 dans un environnement Microsoft 365, Windows/Linux et Veeam Data Cloud.
            </p>
            <ul>
              <li>Durcissement de l’infrastructure Azure avec NSG, restrictions IP et VPN</li>
              <li>Gestion des accès via RBAC, Active Directory et GPO</li>
              <li>Traçabilité et exploitation d’outils multiples en mission 100 % remote</li>
            </ul>
          </article>

          <article class="project">
            <span class="tag">ERGO MADA & Ergo Santé France</span>
            <h3>Pilotage d’infrastructure & support opérationnel</h3>
            <p>
              Coordination IT, administration locale et accompagnement d’environ 80 utilisateurs dans un environnement de production.
            </p>
            <ul>
              <li>Gestion de prestataires externes et coordination avec les équipes France</li>
              <li>Maintien d’un taux de disponibilité de 99,8 %</li>
              <li>Aucun incident majeur de sécurité signalé sur la période</li>
            </ul>
          </article>

          <article class="project">
            <span class="tag">HAITO EURO & HYDROLA France</span>
            <h3>Administration multi-sites & support international</h3>
            <p>
              Optimisation d’une infrastructure IT pour plusieurs entités situées en France, Madagascar, Mexique, Chine et Tunisie.
            </p>
            <ul>
              <li>Support technique niveaux 1 et 2</li>
              <li>Gestion d’accès distants sécurisés</li>
              <li>Maintenance et optimisation du site web via ASP.NET</li>
            </ul>
          </article>

          <article class="project">
            <span class="tag">CREAMATORIUM Fr</span>
            <h3>Design UI/UX d’application mobile</h3>
            <p>
              Conception de wireframes, maquettes et prototypes sur Figma avec documentation détaillée pour l’équipe de développement.
            </p>
            <ul>
              <li>Production d’environ 240 slides de spécifications</li>
              <li>Création de plus de 80 wireframes et 3 prototypes interactifs</li>
              <li>Réduction de 30 % des allers-retours design / développement</li>
            </ul>
          </article>
        </div>
      </div>
    </section>

    <section id="experience">
      <div class="container">
        <div class="section-header">
          <div>
            <div class="mini-title">Parcours</div>
            <h2>Expérience professionnelle</h2>
          </div>
          <p>
            Une progression cohérente entre exploitation IT, administration systèmes, environnements hybrides, support et développement applicatif.
          </p>
        </div>
        <div class="timeline">
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Systems Administrator — UCC EXPERTS France</h3>
                <span>Freelance</span>
              </div>
              <span>Nov. 2025 – Fév. 2026</span>
            </div>
            <p>Mise en conformité ISO 27001, administration Microsoft 365, Windows/Linux, Veeam Data Cloud, sécurisation Azure et gouvernance des accès.</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Designer UI/UX — CREAMATORIUM Fr</h3>
                <span>Freelance</span>
              </div>
              <span>Jan. 2025 – Sept. 2025</span>
            </div>
            <p>Création de wireframes, UI, prototypes interactifs et documentation fonctionnelle pour une application mobile avec collaboration React Native.</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Responsable Informatique — ERGO MADA & Ergo Santé France</h3>
                <span>Infrastructure & support</span>
              </div>
              <span>Mars 2024 – Jan. 2025</span>
            </div>
            <p>Coordination IT, gestion de prestataires, administration locale et maintien d’une infrastructure fiable pour environ 80 utilisateurs.</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Administrateur Systèmes & Réseaux — HAITO EURO & HYDROLA France</h3>
                <span>Multi-sites internationaux</span>
              </div>
              <span>Avr. 2019 – Mars 2024</span>
            </div>
            <p>Amélioration d’infrastructure, support L1/L2, accès distants sécurisés et optimisation du site institutionnel.</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Administrateur Systèmes & Réseaux — SITMA SA Madagascar</h3>
                <span>Environnement hybride</span>
              </div>
              <span>Sept. 2018 – Fév. 2019</span>
            </div>
            <p>Support Windows/Linux/Sage ERP, serveur mail local Linux, contrôleur de domaine Active Directory et formation cybersécurité.</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-top">
              <div>
                <h3>Expériences de stage — ODIENZ Consulting, TEKNET GROUP, YAS, Madagascar Airlines</h3>
                <span>Développement, BI, administration</span>
              </div>
              <span>2013 – 2018</span>
            </div>
            <p>Modules Odoo RH, tableaux de bord BI, ETL Talend, développement Java EE, optimisation systèmes Windows/Linux et documentation technique.</p>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container grid-2">
        <div class="card education">
          <div class="mini-title">Formation</div>
          <h2>Parcours académique</h2>
          <div class="edu-item">
            <h3>Master en Informatique</h3>
            <p style="margin: 0; color: var(--muted);">École Nationale d’Informatique — Université de Fianarantsoa</p>
            <small style="color: var(--muted);">2016 – 2018 • Administration Système & Réseau</small>
          </div>
          <div class="edu-item">
            <h3>Licence en Informatique</h3>
            <p style="margin: 0; color: var(--muted);">École Nationale d’Informatique — Université de Fianarantsoa</p>
            <small style="color: var(--muted);">2012 – 2016 • Génie Logiciel & Gestion de Base de Données</small>
          </div>
          <div class="edu-item">
            <h3>Baccalauréat Scientifique</h3>
            <small style="color: var(--muted);">2010 – 2011</small>
          </div>
        </div>

        <div class="card languages">
          <div class="mini-title">Langues</div>
          <h2>Communication professionnelle</h2>
          <div class="lang-item">
            <h3>Malgache</h3>
            <p style="margin: 0; color: var(--muted);">Langue maternelle</p>
          </div>
          <div class="lang-item">
            <h3>Français</h3>
            <p style="margin: 0; color: var(--muted);">Compétence professionnelle complète</p>
          </div>
          <div class="lang-item">
            <h3>Anglais</h3>
            <p style="margin: 0; color: var(--muted);">Compétence professionnelle</p>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container cta">
        <div>
          <div class="mini-title">Disponible pour</div>
          <h2>Administration systèmes, support IT, sécurisation et exploitation</h2>
          <p>
            Si vous cherchez un profil capable de fiabiliser vos environnements IT, d’accompagner vos utilisateurs et de sécuriser vos infrastructures avec une approche concrète et opérationnelle, parlons-en.
          </p>
        </div>
        <div class="hero-actions" style="margin: 0;">
          <a class="btn btn-primary" href="mailto:zohtiana@gmail.com">Envoyer un email</a>
          <a class="btn btn-secondary" href="tel:+261341985702">Appeler</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>
        © 2026 Zo Haingotiana VOLOLONJANAHARY — Portfolio professionnel en une page, prêt à être déployé sur Netlify, Vercel ou GitHub Pages.
      </p>
    </div>
  </footer>
</body>
</html>
