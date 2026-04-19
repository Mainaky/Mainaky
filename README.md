<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Mainak Roy — GitHub Profile</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet"/>
<style>
  *{box-sizing:border-box;margin:0;padding:0}
  :root{
    --ink:#0a0e1a;--ink2:#2a3050;--ink3:#4a5280;
    --blue:#1A56B0;--blue2:#378ADD;--blue3:#B5D4F4;
    --accent:#D14836;--gold:#EF9F27;
    --surface:#f4f6fb;--card:#ffffff;--line:#e0e6f2;
  }
  body{font-family:'Space Grotesk',sans-serif;background:var(--surface);color:var(--ink);min-height:100vh;overflow-x:hidden}

  /* HERO */
  .hero{background:linear-gradient(135deg,#0a0e1a 0%,#0c1a3a 40%,#1a0a2e 100%);color:#fff;padding:3.5rem 2rem 4rem;text-align:center;position:relative;overflow:hidden}
  .hero::before{content:'';position:absolute;inset:0;background:url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%231A56B0' fill-opacity='0.07'%3E%3Ccircle cx='30' cy='30' r='1.5'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");pointer-events:none}
  .hero-glow{position:absolute;width:500px;height:500px;border-radius:50%;background:radial-gradient(circle,rgba(26,86,176,0.18) 0%,transparent 70%);top:-100px;left:50%;transform:translateX(-50%);pointer-events:none}
  .avatar-ring{width:88px;height:88px;border-radius:50%;background:linear-gradient(135deg,#1A56B0,#378ADD,#D14836);padding:3px;margin:0 auto 1.25rem;animation:spinRing 8s linear infinite}
  @keyframes spinRing{0%{background-position:0%}100%{background-position:360%}}
  .avatar-inner{width:100%;height:100%;border-radius:50%;background:#0c1a3a;display:flex;align-items:center;justify-content:center;font-size:2rem;font-weight:700;color:#378ADD;font-family:'JetBrains Mono',monospace}
  .hero h1{font-size:2.4rem;font-weight:700;letter-spacing:-0.03em;margin-bottom:.3rem;background:linear-gradient(135deg,#fff 0%,#B5D4F4 60%,#378ADD 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
  .hero-sub{font-family:'JetBrains Mono',monospace;font-size:.85rem;color:#378ADD;margin-bottom:1.5rem;letter-spacing:.08em}
  .typing-wrap{height:1.6rem;margin-bottom:2rem;overflow:hidden}
  .typing{font-size:1rem;color:#B5D4F4;font-weight:500;display:inline-block;border-right:2px solid #378ADD;padding-right:4px;animation:blink .75s step-end infinite}
  @keyframes blink{0%,100%{border-color:transparent}50%{border-color:#378ADD}}
  .badges{display:flex;flex-wrap:wrap;gap:.5rem;justify-content:center;margin-bottom:1.5rem}
  .badge{background:rgba(255,255,255,.07);border:1px solid rgba(55,138,221,.3);border-radius:20px;padding:.3rem .85rem;font-size:.78rem;color:#B5D4F4;font-family:'JetBrains Mono',monospace}
  .badge.hot{border-color:rgba(209,72,54,.4);color:#f0997b;background:rgba(209,72,54,.08)}
  .links{display:flex;flex-wrap:wrap;gap:.6rem;justify-content:center}
  .link-btn{display:flex;align-items:center;gap:.4rem;padding:.45rem 1.1rem;border-radius:8px;font-size:.82rem;font-weight:600;text-decoration:none;transition:all .2s}
  .link-btn.primary{background:#1A56B0;color:#fff;border:1px solid #378ADD}
  .link-btn.primary:hover{background:#378ADD;transform:translateY(-2px)}
  .link-btn.ghost{background:rgba(255,255,255,.06);color:#B5D4F4;border:1px solid rgba(255,255,255,.15)}
  .link-btn.ghost:hover{background:rgba(255,255,255,.12);transform:translateY(-2px)}

  /* SECTIONS */
  .section{padding:2.5rem 1.5rem;max-width:900px;margin:0 auto}
  .sec-title{font-size:1.05rem;font-weight:700;color:var(--blue);text-transform:uppercase;letter-spacing:.12em;margin-bottom:1.5rem;display:flex;align-items:center;gap:.6rem}
  .sec-title::after{content:'';flex:1;height:1px;background:var(--line)}

  /* ABOUT */
  .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
  .about-card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:1.1rem 1.25rem;display:flex;gap:.75rem;align-items:flex-start;transition:box-shadow .2s,transform .2s;animation:fadeUp .5s ease both}
  .about-card:hover{box-shadow:0 6px 24px rgba(26,86,176,.1);transform:translateY(-2px)}
  @keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
  .about-icon{width:36px;height:36px;border-radius:8px;background:linear-gradient(135deg,var(--blue3),rgba(26,86,176,.1));display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:1rem}
  .about-label{font-size:.8rem;color:var(--ink3);font-weight:500;margin-bottom:.15rem;font-family:'JetBrains Mono',monospace;letter-spacing:.04em}
  .about-val{font-size:.9rem;color:var(--ink);font-weight:600;line-height:1.3}
  .highlight-tag{display:inline-block;background:linear-gradient(135deg,rgba(26,86,176,.1),rgba(55,138,221,.08));border:1px solid rgba(26,86,176,.2);color:var(--blue);border-radius:6px;padding:.05rem .45rem;font-size:.75rem;font-weight:600;margin-right:.25rem;vertical-align:middle}
  .isro-card{background:linear-gradient(135deg,rgba(239,159,39,.06),rgba(239,159,39,.02));border-color:rgba(239,159,39,.25)!important}
  .research-card{background:linear-gradient(135deg,rgba(26,86,176,.06),rgba(55,138,221,.03));border-color:rgba(26,86,176,.25)!important}

  /* SKILLS */
  .skills-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(170px,1fr));gap:.75rem}
  .skill-group{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:1rem}
  .skill-group-title{font-size:.75rem;font-weight:700;color:var(--blue);text-transform:uppercase;letter-spacing:.1em;margin-bottom:.75rem;font-family:'JetBrains Mono',monospace}
  .skill-pills{display:flex;flex-wrap:wrap;gap:.35rem}
  .pill{background:var(--surface);border:1px solid var(--line);border-radius:20px;padding:.22rem .65rem;font-size:.76rem;font-weight:600;color:var(--ink2);transition:all .2s;cursor:default}
  .pill:hover{background:var(--blue3);border-color:var(--blue2);color:var(--blue)}
  .pill.core{background:rgba(26,86,176,.08);border-color:rgba(26,86,176,.2);color:var(--blue)}
  .pill.hot{background:rgba(209,72,54,.07);border-color:rgba(209,72,54,.2);color:#993C1D}

  /* PROJECTS */
  .projects-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
  .proj-card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:1.4rem;transition:all .25s;position:relative;overflow:hidden;animation:fadeUp .5s ease both}
  .proj-card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;border-radius:14px 14px 0 0}
  .proj-card.blue::before{background:linear-gradient(90deg,#1A56B0,#378ADD)}
  .proj-card.red::before{background:linear-gradient(90deg,#D14836,#f0997b)}
  .proj-card.teal::before{background:linear-gradient(90deg,#0F6E56,#1D9E75)}
  .proj-card.purple::before{background:linear-gradient(90deg,#534AB7,#7F77DD)}
  .proj-card.gold::before{background:linear-gradient(90deg,#BA7517,#EF9F27)}
  .proj-card.green::before{background:linear-gradient(90deg,#3B6D11,#639922)}
  .proj-card:hover{box-shadow:0 8px 32px rgba(26,86,176,.13);transform:translateY(-3px)}
  .proj-header{display:flex;align-items:flex-start;gap:.75rem;margin-bottom:.85rem}
  .proj-icon{width:42px;height:42px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:1.3rem;flex-shrink:0}
  .proj-icon.blue{background:rgba(26,86,176,.1)}
  .proj-icon.red{background:rgba(209,72,54,.1)}
  .proj-icon.teal{background:rgba(15,110,86,.1)}
  .proj-icon.purple{background:rgba(83,74,183,.1)}
  .proj-icon.gold{background:rgba(239,159,39,.1)}
  .proj-icon.green{background:rgba(59,109,17,.1)}
  .proj-name{font-size:1rem;font-weight:700;color:var(--ink);margin-bottom:.2rem}
  .proj-meta{font-size:.75rem;color:var(--ink3);font-family:'JetBrains Mono',monospace}
  .proj-desc{font-size:.83rem;color:var(--ink2);line-height:1.6;margin-bottom:.9rem}
  .proj-stats{display:flex;gap:.75rem;flex-wrap:wrap;margin-bottom:.9rem}
  .proj-stat{background:var(--surface);border-radius:6px;padding:.25rem .6rem;font-size:.76rem;font-weight:700;color:var(--blue);font-family:'JetBrains Mono',monospace}
  .proj-stat.acc{color:#0F6E56;background:rgba(15,110,86,.08)}
  .proj-tags{display:flex;flex-wrap:wrap;gap:.3rem}
  .tag{background:var(--surface);border:1px solid var(--line);border-radius:4px;padding:.18rem .5rem;font-size:.72rem;font-weight:600;color:var(--ink3);font-family:'JetBrains Mono',monospace}

  /* ACHIEVEMENTS */
  .ach-list{display:flex;flex-direction:column;gap:.75rem}
  .ach-item{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:1rem 1.25rem;display:flex;align-items:center;gap:1rem;transition:all .2s;animation:fadeUp .5s ease both}
  .ach-item:hover{box-shadow:0 4px 16px rgba(26,86,176,.09);transform:translateX(4px)}
  .ach-year{font-family:'JetBrains Mono',monospace;font-size:.78rem;font-weight:700;color:var(--blue);background:rgba(26,86,176,.07);border-radius:6px;padding:.2rem .6rem;flex-shrink:0;min-width:52px;text-align:center}
  .ach-content{flex:1}
  .ach-title{font-size:.9rem;font-weight:700;color:var(--ink);margin-bottom:.15rem}
  .ach-sub{font-size:.78rem;color:var(--ink3)}
  .ach-badge{padding:.2rem .6rem;border-radius:20px;font-size:.7rem;font-weight:700;flex-shrink:0}
  .ach-badge.paper{background:rgba(26,86,176,.09);color:var(--blue);border:1px solid rgba(26,86,176,.2)}
  .ach-badge.isro{background:rgba(239,159,39,.1);color:#BA7517;border:1px solid rgba(239,159,39,.3)}
  .ach-badge.cert{background:rgba(15,110,86,.09);color:#0F6E56;border:1px solid rgba(15,110,86,.2)}
  .ach-badge.club{background:rgba(83,74,183,.09);color:#534AB7;border:1px solid rgba(83,74,183,.2)}

  /* STATS */
  .stats-row{display:flex;flex-wrap:wrap;gap:1rem;justify-content:center}
  .stat-card{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:1rem 1.5rem;text-align:center;flex:1;min-width:130px}
  .stat-num{font-size:2rem;font-weight:700;color:var(--blue);font-family:'JetBrains Mono',monospace;line-height:1}
  .stat-lbl{font-size:.75rem;color:var(--ink3);margin-top:.3rem;font-weight:600;text-transform:uppercase;letter-spacing:.08em}
  .github-imgs{display:flex;flex-wrap:wrap;gap:.75rem;justify-content:center;margin-top:1.25rem}
  .github-imgs img{border-radius:10px;max-width:100%;border:1px solid var(--line)}

  /* COURSES */
  .courses-wrap{display:flex;flex-wrap:wrap;gap:.45rem}
  .course{background:var(--card);border:1px solid var(--line);border-radius:8px;padding:.35rem .8rem;font-size:.8rem;font-weight:500;color:var(--ink2)}

  /* FOOTER */
  .footer{background:linear-gradient(135deg,#0a0e1a,#0c1a3a);color:#B5D4F4;text-align:center;padding:2.5rem 1.5rem;margin-top:1rem}
  .footer-name{font-size:1.4rem;font-weight:700;color:#fff;margin-bottom:.4rem;font-family:'JetBrains Mono',monospace}
  .footer-open{display:inline-flex;align-items:center;gap:.5rem;background:rgba(26,86,176,.25);border:1px solid rgba(55,138,221,.3);border-radius:20px;padding:.4rem 1rem;margin:.75rem auto;font-size:.82rem;color:#B5D4F4}
  .open-dot{width:8px;height:8px;border-radius:50%;background:#1D9E75;animation:pulse 1.5s ease-in-out infinite}
  @keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.6;transform:scale(.8)}}
  .footer-links{display:flex;flex-wrap:wrap;gap:.6rem;justify-content:center;margin-top:1rem}
  .foot-link{color:#378ADD;font-size:.82rem;text-decoration:none;padding:.25rem .65rem;border-radius:6px;border:1px solid rgba(55,138,221,.2);transition:all .2s}
  .foot-link:hover{background:rgba(55,138,221,.15)}

  /* DIVIDER */
  .divider{height:1px;background:linear-gradient(90deg,transparent,var(--line),transparent);margin:0 1.5rem}

  @media(max-width:600px){
    .about-grid,.projects-grid{grid-template-columns:1fr}
    .hero h1{font-size:1.8rem}
  }
</style>
</head>
<body>

<div class="hero">
  <div class="hero-glow"></div>
  <div class="avatar-ring">
    <div class="avatar-inner">MR</div>
  </div>
  <h1>Mainak Roy</h1>
  <div class="hero-sub">B.Tech CSE (Data Science) · NIIT University · 2023–2027</div>
  <div class="typing-wrap">
    <span class="typing" id="typer">Building systems that think.</span>
  </div>
  <div class="badges">
    <span class="badge">Machine Learning</span>
    <span class="badge">Agentic AI</span>
    <span class="badge">Medical Imaging</span>
    <span class="badge">MLOps</span>
    <span class="badge hot">ICICV 2026 — Published</span>
    <span class="badge hot">ISRO Hackathon 2025</span>
  </div>
  <div class="links">
    <a class="link-btn primary" href="https://www.linkedin.com/in/mainak-roy-7415b2258/" target="_blank">LinkedIn</a>
    <a class="link-btn primary" href="https://mainak-portfolio-dvn2.vercel.app/" target="_blank">Portfolio</a>
    <a class="link-btn ghost" href="mailto:mainak.roy23@st.niituniversity.in">Email</a>
    <a class="link-btn ghost" href="https://github.com/Mainaky" target="_blank">GitHub</a>
  </div>
</div>

<div class="section">
  <div class="sec-title">About Me</div>
  <div class="about-grid">
    <div class="about-card" style="animation-delay:.05s">
      <div class="about-icon">🎓</div>
      <div><div class="about-label">Education</div><div class="about-val">B.Tech CSE <span class="highlight-tag">Data Science</span><br>NIIT University, Neemrana · 2023–2027</div></div>
    </div>
    <div class="about-card" style="animation-delay:.1s">
      <div class="about-icon">📍</div>
      <div><div class="about-label">Based in</div><div class="about-val">Kolkata, West Bengal, India 🇮🇳</div></div>
    </div>
    <div class="about-card" style="animation-delay:.15s">
      <div class="about-icon">🤖</div>
      <div><div class="about-label">Core focus</div><div class="about-val">ML Pipelines · <span class="highlight-tag">Agentic AI</span> · Medical Imaging<br><span style="font-size:.8rem;color:var(--ink3)">LangChain · LangGraph · RAG · Multi-Agent Orchestration</span></div></div>
    </div>
    <div class="about-card" style="animation-delay:.2s">
      <div class="about-icon">⚙️</div>
      <div><div class="about-label">MLOps & Cloud</div><div class="about-val">Docker · Jenkins · CI/CD · MLflow<br><span style="font-size:.8rem;color:var(--ink3)">AWS (EC2, S3, Lambda) · Snowflake · HDFS</span></div></div>
    </div>
    <div class="about-card research-card" style="animation-delay:.25s">
      <div class="about-icon">📄</div>
      <div><div class="about-label">Research</div><div class="about-val"><span class="highlight-tag">ICICV 2026</span> Accepted<br><span style="font-size:.8rem;color:var(--ink3)">Maze Solving Algorithms in Known & Unknown Environments</span></div></div>
    </div>
    <div class="about-card isro-card" style="animation-delay:.3s">
      <div class="about-icon">🛸</div>
      <div><div class="about-label">National Recognition</div><div class="about-val">ISRO Bharatiya Antariksh Hackathon 2025<br><span style="font-size:.8rem;color:var(--ink3)">Certificate of Acknowledgement · AI Air Quality System</span></div></div>
    </div>
    <div class="about-card" style="animation-delay:.35s">
      <div class="about-icon">🧮</div>
      <div><div class="about-label">Leadership</div><div class="about-val">Club Coordinator<br><span style="font-size:.8rem;color:var(--ink3)">Ramanujan Mathematics Club, NIIT University · 2025–2026</span></div></div>
    </div>
    <div class="about-card" style="animation-delay:.4s">
      <div class="about-icon">💼</div>
      <div><div class="about-label">Open to</div><div class="about-val">Internships · Research Collaborations · Open Source</div></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sec-title">Tech Stack</div>
  <div class="skills-grid">
    <div class="skill-group">
      <div class="skill-group-title">Languages</div>
      <div class="skill-pills">
        <span class="pill core">Python</span><span class="pill core">C#</span><span class="pill">SQL</span><span class="pill">Bash</span><span class="pill">R</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">ML & AI</div>
      <div class="skill-pills">
        <span class="pill core">TensorFlow</span><span class="pill core">PyTorch</span><span class="pill">scikit-learn</span><span class="pill">XGBoost</span><span class="pill">U-Net</span><span class="pill">Grad-CAM</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">Agentic & Gen AI</div>
      <div class="skill-pills">
        <span class="pill hot">LangChain</span><span class="pill hot">LangGraph</span><span class="pill hot">RAG</span><span class="pill">Google Gemini</span><span class="pill">FastAPI</span><span class="pill">Multi-Agent</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">MLOps & DevOps</div>
      <div class="skill-pills">
        <span class="pill core">Docker</span><span class="pill core">Jenkins</span><span class="pill">MLflow</span><span class="pill">CI/CD</span><span class="pill">GitHub Actions</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">Cloud & Big Data</div>
      <div class="skill-pills">
        <span class="pill">AWS EC2</span><span class="pill">S3</span><span class="pill">Lambda</span><span class="pill core">Snowflake</span><span class="pill">HDFS</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">Databases & Viz</div>
      <div class="skill-pills">
        <span class="pill">PostgreSQL</span><span class="pill">MySQL</span><span class="pill">MongoDB</span><span class="pill">Streamlit</span><span class="pill">Matplotlib</span><span class="pill">Seaborn</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-title">Desktop & UI</div>
      <div class="skill-pills">
        <span class="pill core">WPF</span><span class="pill core">.NET 8</span><span class="pill">Win32 API</span><span class="pill">XAML</span>
      </div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sec-title">Featured Projects</div>
  <div class="projects-grid">

    <div class="proj-card blue" style="animation-delay:.05s">
      <div class="proj-header">
        <div class="proj-icon blue">🧠</div>
        <div>
          <div class="proj-name">NeuroSeg</div>
          <div class="proj-meta">Brain Tumour Detection & Segmentation</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">97.2% Seg Acc</span>
        <span class="proj-stat acc">99.1% Class Acc</span>
      </div>
      <div class="proj-desc">U-Net CNN for MRI segmentation with VGG19 transfer learning, Grad-CAM clinical explainability, and full CI/CD pipeline via GitHub → Jenkins → Docker → DockerHub. Outperforms ANN (82.4%) and Standard CNN (94.8%).</div>
      <div class="proj-tags">
        <span class="tag">TensorFlow</span><span class="tag">U-Net</span><span class="tag">VGG19</span><span class="tag">Grad-CAM</span><span class="tag">Docker</span><span class="tag">Jenkins</span><span class="tag">Medical AI</span>
      </div>
    </div>

    <div class="proj-card teal" style="animation-delay:.1s">
      <div class="proj-header">
        <div class="proj-icon teal">📍</div>
        <div>
          <div class="proj-name">ZonePulse</div>
          <div class="proj-meta">Ride Demand Prediction & Analytics</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">4.7M+ Records</span>
        <span class="proj-stat acc">78% R²</span>
      </div>
      <div class="proj-desc">Geospatial ride demand forecasting over 4.7M trip records via Snowflake cloud DW. XGBoost + Random Forest pipeline with Streamlit dashboards, surge pricing strategy, and 5 PM peak detection.</div>
      <div class="proj-tags">
        <span class="tag">XGBoost</span><span class="tag">Snowflake</span><span class="tag">Streamlit</span><span class="tag">Random Forest</span><span class="tag">SQL</span>
      </div>
    </div>

    <div class="proj-card red" style="animation-delay:.15s">
      <div class="proj-header">
        <div class="proj-icon red">🏥</div>
        <div>
          <div class="proj-name">MedMes / CareFlow</div>
          <div class="proj-meta">Healthcare Multi-Agent AI System</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">4-Agent System</span>
        <span class="proj-stat acc">15 Clinical Guidelines</span>
      </div>
      <div class="proj-desc">4-agent orchestration (Navigator, Coordinator, Quality Analyst, AI Nurse) with RAG grounded on ADA/AHA/KDIGO guidelines, FHIR-compatible synthetic patient data, real-time routing confidence tracking.</div>
      <div class="proj-tags">
        <span class="tag">LangChain</span><span class="tag">Gemini 1.5</span><span class="tag">FastAPI</span><span class="tag">RAG</span><span class="tag">FHIR</span><span class="tag">MLOps</span>
      </div>
    </div>

    <div class="proj-card purple" style="animation-delay:.2s">
      <div class="proj-header">
        <div class="proj-icon purple">🖥️</div>
        <div>
          <div class="proj-name">SwiftDesk</div>
          <div class="proj-meta">Windows App Launcher · Spotlight-style</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">Alt+Space Global</span>
        <span class="proj-stat acc">Multi-monitor DPI</span>
      </div>
      <div class="proj-desc">macOS Spotlight-inspired Windows launcher with global hotkey via Win32 P/Invoke, async multi-provider search with CancellationToken, Start Menu indexing, math eval, clipboard, and C# 9 immutable models.</div>
      <div class="proj-tags">
        <span class="tag">C#</span><span class="tag">WPF</span><span class="tag">.NET 8</span><span class="tag">Win32 API</span><span class="tag">XAML</span>
      </div>
    </div>

    <div class="proj-card gold" style="animation-delay:.25s">
      <div class="proj-header">
        <div class="proj-icon gold">🛸</div>
        <div>
          <div class="proj-name">ISRO Air Quality AI</div>
          <div class="proj-meta">Bharatiya Antariksh Hackathon 2025</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">ISRO Certified</span>
      </div>
      <div class="proj-desc">AI-based air pollution monitoring & forecasting system built for ISRO Bharatiya Antariksh Hackathon 2025. Received official ISRO Certificate of Acknowledgement for national-level recognition.</div>
      <div class="proj-tags">
        <span class="tag">Python</span><span class="tag">Forecasting</span><span class="tag">ML</span><span class="tag">Remote Sensing</span>
      </div>
    </div>

    <div class="proj-card green" style="animation-delay:.3s">
      <div class="proj-header">
        <div class="proj-icon green">🔬</div>
        <div>
          <div class="proj-name">Maze Solver Study</div>
          <div class="proj-meta">ICICV 2026 — Research Paper</div>
        </div>
      </div>
      <div class="proj-stats">
        <span class="proj-stat acc">Published</span>
      </div>
      <div class="proj-desc">Comparative experimental study of maze-solving algorithms in known vs unknown environments. Accepted at ICICV 2026 — International Conference on Innovative Computing & Communications. BFS, DFS, A*, Q-Learning analysis.</div>
      <div class="proj-tags">
        <span class="tag">BFS</span><span class="tag">DFS</span><span class="tag">A*</span><span class="tag">Q-Learning</span><span class="tag">Research</span>
      </div>
    </div>

  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sec-title">GitHub Stats</div>
  <div class="stats-row">
    <div class="stat-card"><div class="stat-num">12+</div><div class="stat-lbl">Repositories</div></div>
    <div class="stat-card"><div class="stat-num">6</div><div class="stat-lbl">Major Projects</div></div>
    <div class="stat-card"><div class="stat-num">1</div><div class="stat-lbl">Research Paper</div></div>
    <div class="stat-card"><div class="stat-num">4+</div><div class="stat-lbl">Years Active</div></div>
  </div>
  <div class="github-imgs">
    <img src="https://github-readme-stats.vercel.app/api?username=Mainaky&show_icons=true&hide_border=true&title_color=1A56B0&icon_color=378ADD&text_color=2a3050&bg_color=ffffff&count_private=true" height="160" alt="GitHub Stats"/>
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Mainaky&layout=compact&hide_border=true&title_color=1A56B0&text_color=2a3050&bg_color=ffffff" height="160" alt="Top Languages"/>
  </div>
  <div class="github-imgs" style="margin-top:.75rem">
    <img src="https://streak-stats.demolab.com?user=Mainaky&hide_border=true&ring=1A56B0&fire=D14836&currStreakLabel=1A56B0&sideLabels=2a3050&dates=888888&background=ffffff" height="140" alt="Streak Stats"/>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sec-title">Achievements & Certifications</div>
  <div class="ach-list">
    <div class="ach-item" style="animation-delay:.05s">
      <div class="ach-year">2026</div>
      <div class="ach-content">
        <div class="ach-title">ICICV 2026 Research Paper Accepted</div>
        <div class="ach-sub">A Comparative Experimental Study of Maze Solving Algorithms in Known and Unknown Environments · International Conference on Innovative Computing & Communications</div>
      </div>
      <span class="ach-badge paper">Research</span>
    </div>
    <div class="ach-item" style="animation-delay:.1s">
      <div class="ach-year">2025</div>
      <div class="ach-content">
        <div class="ach-title">ISRO Bharatiya Antariksh Hackathon 2025</div>
        <div class="ach-sub">AI Air Pollution Monitoring & Forecasting System · Certificate of Acknowledgement from ISRO</div>
      </div>
      <span class="ach-badge isro">ISRO</span>
    </div>
    <div class="ach-item" style="animation-delay:.15s">
      <div class="ach-year">2025</div>
      <div class="ach-content">
        <div class="ach-title">LetsUpgrade Certification</div>
        <div class="ach-sub">Build RAG Chatbot with Python · May 2025</div>
      </div>
      <span class="ach-badge cert">Certified</span>
    </div>
    <div class="ach-item" style="animation-delay:.2s">
      <div class="ach-year">2025–26</div>
      <div class="ach-content">
        <div class="ach-title">Club Coordinator — Ramanujan Mathematics Club</div>
        <div class="ach-sub">NIIT University · Academic Year 2025–2026</div>
      </div>
      <span class="ach-badge club">Leadership</span>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sec-title">Relevant Coursework</div>
  <div class="courses-wrap">
    <span class="course">Predictive Modeling for Data Science</span>
    <span class="course">Numerical Methods for Data Science</span>
    <span class="course">Inferential Statistics</span>
    <span class="course">Big Data Concepts</span>
    <span class="course">Artificial Intelligence</span>
    <span class="course">Object Oriented Programming</span>
  </div>
</div>

<div class="footer">
  <div class="footer-name">Mainak Roy</div>
  <div style="font-size:.85rem;margin-bottom:.5rem">B.Tech CSE (Data Science) · NIIT University · Kolkata, India</div>
  <div style="display:flex;justify-content:center">
    <div class="footer-open"><span class="open-dot"></span> Open to Internships, Research & Open Source</div>
  </div>
  <div class="footer-links">
    <a class="foot-link" href="https://www.linkedin.com/in/mainak-roy-7415b2258/" target="_blank">LinkedIn</a>
    <a class="foot-link" href="https://mainak-portfolio-dvn2.vercel.app/" target="_blank">Portfolio</a>
    <a class="foot-link" href="mailto:mainak.roy23@st.niituniversity.in">Email</a>
    <a class="foot-link" href="https://github.com/Mainaky" target="_blank">GitHub</a>
  </div>
  <div style="margin-top:1.5rem;font-size:.72rem;color:rgba(181,212,244,.4);font-family:'JetBrains Mono',monospace">Built with precision · Powered by purpose</div>
</div>

<script>
const lines = [
  "Building systems that think.",
  "ML · Agentic AI · Medical Imaging",
  "Research @ ICICV 2026.",
  "ISRO Hackathon Acknowledged.",
  "Open to Internships & Research.",
];
let li = 0, ci = 0, del = false;
const el = document.getElementById('typer');
function tick() {
  const txt = lines[li];
  if (!del) {
    ci++;
    el.textContent = txt.slice(0, ci);
    if (ci === txt.length) { del = true; setTimeout(tick, 2200); return; }
  } else {
    ci--;
    el.textContent = txt.slice(0, ci);
    if (ci === 0) { del = false; li = (li + 1) % lines.length; setTimeout(tick, 300); return; }
  }
  setTimeout(tick, del ? 40 : 65);
}
tick();
</script>

</body>
</html>
