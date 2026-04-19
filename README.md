<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Mainak Roy | Data Scientist & AI Engineer</title>
  <!-- Google Fonts & Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <!-- AOS CSS (Animate on Scroll) -->
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: #f9fbfd;
      color: #1e293b;
      scroll-behavior: smooth;
      overflow-x: hidden;
    }

    /* custom scrollbar */
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #eef2f6;
    }
    ::-webkit-scrollbar-thumb {
      background: #1A56B0;
      border-radius: 12px;
    }

    /* wave animations & containers */
    .wave-header {
      background: linear-gradient(135deg, #0b2b5c 0%, #1A56B0 100%);
      position: relative;
      overflow: hidden;
    }

    .glass-card {
      background: rgba(255, 255, 255, 0.9);
      backdrop-filter: blur(2px);
      border-radius: 2rem;
      box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.08), 0 0 0 1px rgba(0, 0, 0, 0.02);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .glass-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 28px 40px -16px rgba(26,86,176,0.2), 0 0 0 1px rgba(26,86,176,0.1);
    }

    .badge-skill {
      background: #eef3ff;
      color: #1A56B0;
      font-weight: 500;
      border-radius: 40px;
      padding: 0.35rem 1rem;
      font-size: 0.8rem;
      transition: all 0.2s;
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }
    .badge-skill i {
      font-size: 0.8rem;
    }

    .project-card {
      background: white;
      border-radius: 1.5rem;
      padding: 1.5rem;
      height: 100%;
      transition: all 0.3s cubic-bezier(0.2, 0.9, 0.4, 1.1);
      border: 1px solid rgba(0,0,0,0.05);
    }
    .project-card:hover {
      border-color: #1A56B030;
      box-shadow: 0 20px 30px -12px rgba(0,0,0,0.1);
    }

    .tech-tag {
      background: #f1f5f9;
      border-radius: 20px;
      padding: 0.2rem 0.75rem;
      font-size: 0.7rem;
      font-weight: 500;
      color: #0f3b6f;
    }

    .stat-gradient {
      background: linear-gradient(145deg, #ffffff, #f5f9ff);
    }

    .btn-outline-primary {
      border: 1.5px solid #1A56B0;
      background: transparent;
      color: #1A56B0;
      border-radius: 40px;
      padding: 0.5rem 1.4rem;
      font-weight: 600;
      transition: 0.2s;
    }
    .btn-outline-primary:hover {
      background: #1A56B0;
      color: white;
      transform: scale(0.97);
    }

    .achievement-row {
      background: #ffffffd9;
      border-radius: 1.2rem;
      padding: 1rem;
      margin-bottom: 0.8rem;
      border-left: 5px solid #1A56B0;
    }

    footer {
      background: #0f172a;
    }

    @keyframes float {
      0% { transform: translateY(0px); }
      100% { transform: translateY(-6px); }
    }
    .float-animation {
      animation: float 4s ease-in-out infinite;
    }
  </style>
</head>
<body>

<!-- animated header with waves -->
<div class="wave-header" style="padding: 1rem 0 0 0; position: relative;">
  <div style="position: relative; z-index: 3; text-align: center; padding: 2rem 1rem 1rem;">
    <div data-aos="fade-up">
      <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=34&duration=2800&pause=800&color=FFFFFF&center=true&vCenter=true&width=800&lines=Hey+there%2C+I'm+Mainak+Roy+%F0%9F%91%8B;Data+Science+%7C+ML+%7C+Agentic+AI;Medical+Imaging+%7C+MLOps+%7C+Desktop+Tools;Building+systems+that+think." alt="Typing SVG" style="max-width:100%">
    </div>
    <div class="mt-4 d-flex flex-wrap justify-content-center gap-3" data-aos="fade-up" data-aos-delay="100">
      <span class="badge-skill" style="background:#ffffff22; color:white; backdrop-filter: blur(4px);"><i class="fas fa-graduation-cap"></i> B.Tech CSE (Data Science) · NIIT University</span>
      <span class="badge-skill" style="background:#ffffff22; color:white;"><i class="fas fa-map-marker-alt"></i> Kolkata, India</span>
      <span class="badge-skill" style="background:#ffffff22; color:white;"><i class="fas fa-chart-line"></i> CGPA: 9.17</span>
    </div>
    <div class="mt-4 d-flex flex-wrap justify-content-center gap-3" data-aos="fade-up" data-aos-delay="200">
      <a href="https://www.linkedin.com/in/mainak-roy-7415b2258/" target="_blank" class="btn-outline-primary" style="background: white; color:#1A56B0;"><i class="fab fa-linkedin"></i> LinkedIn</a>
      <a href="https://mainak-portfolio-dvn2.vercel.app/" target="_blank" class="btn-outline-primary" style="background: white; color:#1A56B0;"><i class="fas fa-globe"></i> Portfolio</a>
      <a href="mailto:mainak.roy23@st.niituniversity.in" class="btn-outline-primary" style="background: white; color:#1A56B0;"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://github.com/Mainaky" target="_blank" class="btn-outline-primary" style="background: white; color:#1A56B0;"><i class="fab fa-github"></i> GitHub</a>
    </div>
    <div class="mt-3" data-aos="fade-up" data-aos-delay="300">
      <img src="https://komarev.com/ghpvc/?username=Mainaky&style=flat-square&color=ffffff&label=PROFILE+VIEWS" alt="views" style="filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1));">
    </div>
  </div>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 120" style="display: block; width: 100%; margin-bottom: -6px;">
    <path fill="#f9fbfd" fill-opacity="1" d="M0,64L48,69.3C96,75,192,85,288,80C384,75,480,53,576,53.3C672,53,768,75,864,90.7C960,107,1056,117,1152,112C1248,107,1344,85,1392,74.7L1440,64L1440,120L1392,120C1344,120,1248,120,1152,120C1056,120,960,120,864,120C768,120,672,120,576,120C480,120,384,120,288,120C192,120,96,120,48,120L0,120Z"></path>
  </svg>
</div>

<main class="container" style="max-width: 1300px; margin: 0 auto; padding: 1.5rem 2rem 3rem;">
  
  <!-- about me + sophisticated skills -->
  <div class="row g-5 align-items-start" style="display: flex; flex-wrap: wrap; gap: 2rem; margin-bottom: 4rem;">
    <div class="col-md-7" data-aos="fade-right" style="flex: 1.5; min-width: 260px;">
      <div class="glass-card p-4 p-xl-5 h-100">
        <div class="d-flex align-items-center gap-3 mb-3">
          <i class="fas fa-user-astronaut" style="font-size: 2.5rem; color:#1A56B0;"></i>
          <h2 class="fw-bold" style="color: #0c2d5a;">🧠 About Me</h2>
        </div>
        <p class="fs-5 fw-semibold">Mainak Roy — B.Tech CSE (Data Science) @ NIIT University, Neemrana (2023–2027)</p>
        <div class="mb-3 d-flex flex-wrap gap-2">
          <span class="badge-skill"><i class="fas fa-code"></i> DSA & OOP</span>
          <span class="badge-skill"><i class="fas fa-brain"></i> Agentic AI</span>
          <span class="badge-skill"><i class="fas fa-microscope"></i> Medical Imaging</span>
          <span class="badge-skill"><i class="fas fa-cloud-upload-alt"></i> MLOps</span>
          <span class="badge-skill"><i class="fas fa-robot"></i> LangGraph/RAG</span>
        </div>
        <ul class="list-unstyled" style="line-height: 1.6;">
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> <strong>Scalable backend systems & real-time apps</strong> — AWS, Docker, CI/CD pipelines</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> <strong>ML, RAG & Multi-Agent Orchestration</strong> — LangChain, LangGraph, Gemini 1.5 Flash</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> <strong>Research paper accepted @ ICICV 2026</strong> — Maze Solving Algorithms (Known vs Unknown)</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> <strong>ISRO Bharatiya Antariksh Hackathon 2025</strong> — Certificate of Acknowledgement</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> 📜 Certified: Build RAG Chatbot with Python — LetsUpgrade ✅ (May 2025)</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> 🧮 Club Coordinator — Ramanujan Mathematics Club, NIIT University (2025–2026)</li>
          <li class="mb-2"><i class="fas fa-check-circle text-primary me-2"></i> Mentored 20+ students in DSA, Python & ML — fostering practical coding skills</li>
          <li class="mb-2"><i class="fas fa-chalkboard-user text-primary me-2"></i> Fun fact: I explain neural networks to math students for fun 😄</li>
        </ul>
        <div class="mt-3 pt-2">
          <i class="fas fa-map-pin text-secondary"></i> <span class="fw-semibold">📍 Kolkata, West Bengal, India | Open to Internships & Research Collaborations</span>
        </div>
      </div>
    </div>
    <div class="col-md-4" data-aos="fade-left" style="flex: 1; min-width: 260px;">
      <div class="glass-card p-4 h-100">
        <h3 class="fw-bold mb-3"><i class="fas fa-tachometer-alt"></i> Core Competencies</h3>
        <div class="d-flex flex-wrap gap-2 mb-4">
          <span class="badge-skill">Python</span><span class="badge-skill">SQL</span><span class="badge-skill">C# / .NET</span>
          <span class="badge-skill">TensorFlow</span><span class="badge-skill">PyTorch</span><span class="badge-skill">Scikit-learn</span>
          <span class="badge-skill">LangChain</span><span class="badge-skill">FastAPI</span><span class="badge-skill">Docker</span>
          <span class="badge-skill">Jenkins</span><span class="badge-skill">AWS (EC2,S3,Lambda)</span><span class="badge-skill">Snowflake</span>
          <span class="badge-skill">Streamlit</span><span class="badge-skill">WPF</span><span class="badge-skill">MLflow</span>
        </div>
        <hr>
        <h4 class="fw-semibold fs-5"><i class="fas fa-certificate"></i> Certifications & Awards</h4>
        <div class="mt-2 small">
          <p><i class="fas fa-trophy text-warning"></i> <strong>ICICV 2026</strong> — Research Paper Acceptance (Maze Solving)</p>
          <p><i class="fas fa-space-shuttle text-info"></i> <strong>ISRO Hackathon 2025</strong> — Air Quality AI & Certificate of Acknowledgement</p>
          <p><i class="fas fa-graduation-cap"></i> <strong>LetsUpgrade</strong> — Build RAG Chatbot with Python (May 2025)</p>
        </div>
        <div class="mt-3">
          <div class="progress mb-2" style="height: 8px; border-radius: 10px; background:#e2e8f0;">
            <div class="progress-bar bg-primary" style="width: 92%; border-radius:10px;" aria-valuenow="92"></div>
          </div>
          <p class="mb-0 fw-semibold">Passion for Agentic AI & MLOps <i class="fas fa-fire"></i></p>
        </div>
      </div>
    </div>
  </div>

  <!-- featured projects heading -->
  <div class="mt-5 mb-4 text-center" data-aos="fade-up">
    <h2 class="display-6 fw-bold" style="color:#1A56B0;">🚀 Featured Projects</h2>
    <p class="text-secondary">Cutting-edge systems — Medical AI, MLOps, Agentic workflows & high-performance apps</p>
  </div>

  <!-- projects grid (2x2 then 2) -->
  <div class="row g-4">
    <!-- project 1 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="50">
      <div class="project-card">
        <div class="d-flex justify-content-between align-items-start">
          <h3 class="fw-bold fs-4">🧠 NeuroSeg — Brain Tumour Detection</h3>
          <span class="tech-tag">Medical Imaging</span>
        </div>
        <p class="mt-2">U-Net CNN for MRI segmentation → 97.2% accuracy | VGG19 Transfer Learning → 99.1% classification. Grad-CAM explainability, full CI/CD: GitHub → Jenkins → Docker → DockerHub.</p>
        <div class="d-flex flex-wrap gap-2 mt-2 mb-2">
          <span class="tech-tag">TensorFlow</span><span class="tech-tag">U-Net</span><span class="tech-tag">VGG19</span><span class="tech-tag">Grad-CAM</span><span class="tech-tag">Docker</span><span class="tech-tag">Jenkins</span>
        </div>
        <div class="mt-3"><i class="fas fa-chart-line text-primary"></i> Outperforms ANN (82.4%) & Standard CNN (94.8%)</div>
      </div>
    </div>
    <!-- project 2 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="100">
      <div class="project-card">
        <h3 class="fw-bold fs-4">📍 ZonePulse — Ride Demand Prediction</h3>
        <p>Processes 4.7M+ trip records via Snowflake cloud DW. XGBoost + Random Forest → 78% variance explained. Geospatial heatmaps with Streamlit dashboards, identifies peak demand windows for surge pricing.</p>
        <div class="d-flex flex-wrap gap-2 mt-2 mb-2">
          <span class="tech-tag">Python</span><span class="tech-tag">XGBoost</span><span class="tech-tag">Snowflake</span><span class="tech-tag">Streamlit</span><span class="tech-tag">SQL</span>
        </div>
        <div class="mt-2"><i class="fas fa-chart-simple"></i> Critical 5 PM peak demand windows & driver allocation</div>
      </div>
    </div>
    <!-- project 3 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="150">
      <div class="project-card">
        <h3 class="fw-bold fs-4">🏥 MedMes / CareFlow — Healthcare AI</h3>
        <p>4-agent system: Navigator, Coordinator, Quality Analyst, AI Nurse. RAG pipeline grounded on 15 clinical guidelines (ADA, AHA, KDIGO). FHIR-compatible synthetic data, real-time evaluation latency tracking.</p>
        <div class="d-flex flex-wrap gap-2 mt-2">
          <span class="tech-tag">LangChain</span><span class="tech-tag">Google Gemini 1.5 Flash</span><span class="tech-tag">FastAPI</span><span class="tech-tag">RAG</span><span class="tech-tag">LangGraph</span>
        </div>
      </div>
    </div>
    <!-- project 4 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="200">
      <div class="project-card">
        <h3 class="fw-bold fs-4">🖥️ SwiftDesk — Windows App Launcher</h3>
        <p>macOS Spotlight-style launcher for Windows. Global Alt+Space hotkey (Win32 P/Invoke), async multi-provider search, Start Menu indexing, file search, math evaluation & clipboard. DPI-aware multi-monitor support, C# 9 immutable models.</p>
        <div class="d-flex flex-wrap gap-2 mt-2">
          <span class="tech-tag">C#</span><span class="tech-tag">WPF</span><span class="tech-tag">.NET 8</span><span class="tech-tag">Win32 API</span>
        </div>
      </div>
    </div>
    <!-- project 5 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="250">
      <div class="project-card">
        <h3 class="fw-bold fs-4">🛸 ISRO Air Quality AI — Hackathon 2025</h3>
        <p>AI-based air pollution monitoring & forecasting system built for ISRO Bharatiya Antariksh Hackathon 2025. Received prestigious ISRO Certificate of Acknowledgement. Machine learning forecasting for pollutants.</p>
        <div class="d-flex flex-wrap gap-2"><span class="tech-tag">Python</span><span class="tech-tag">Forecasting</span><span class="tech-tag">ML</span><span class="tech-tag">ISRO</span></div>
      </div>
    </div>
    <!-- project 6 -->
    <div class="col-md-6 col-lg-6" data-aos="zoom-in" data-aos-delay="300">
      <div class="project-card">
        <h3 class="fw-bold fs-4">🔬 Maze Solver — ICICV 2026 Research</h3>
        <p>Comparative study: maze-solving algorithms in known vs unknown environments. BFS, DFS, A*, Q-Learning analysis. Accepted at International Conference on Innovative Computing & Communications (ICICV 2026).</p>
        <div class="d-flex flex-wrap gap-2"><span class="tech-tag">Python</span><span class="tech-tag">AI Search</span><span class="tech-tag">Q-Learning</span><span class="tech-tag">Research</span></div>
      </div>
    </div>
  </div>

  <!-- achievements & research publication table -->
  <div class="mt-5 pt-4" data-aos="fade-up">
    <div class="glass-card p-4">
      <h2 class="fw-bold mb-4"><i class="fas fa-medal"></i> 🏆 Achievements & Research Excellence</h2>
      <div class="achievement-row d-flex flex-wrap justify-content-between align-items-center">
        <div><strong>📄 ICICV 2026</strong> — Research Paper Accepted</div>
        <div class="text-secondary">"A Comparative Experimental Study of Maze Solving Algorithms in Known and Unknown Environments"</div>
      </div>
      <div class="achievement-row d-flex flex-wrap justify-content-between align-items-center">
        <div><strong>🛸 ISRO Bharatiya Antariksh Hackathon 2025</strong></div>
        <div class="text-secondary">AI Air Pollution Monitoring & Forecasting — Certificate of Acknowledgement</div>
      </div>
      <div class="achievement-row d-flex flex-wrap justify-content-between align-items-center">
        <div><strong>🎓 LetsUpgrade Certification</strong></div>
        <div class="text-secondary">Build RAG Chatbot with Python (May 2025) ✅</div>
      </div>
      <div class="achievement-row d-flex flex-wrap justify-content-between align-items-center">
        <div><strong>🧮 Club Coordinator</strong></div>
        <div class="text-secondary">Ramanujan Mathematics Club, NIIT University (2025–2026) — led math & coding events</div>
      </div>
      <div class="achievement-row d-flex flex-wrap justify-content-between align-items-center">
        <div><strong>🏅 Mentorship</strong></div>
        <div class="text-secondary">Mentored 20+ students in DSA, Python & ML — boosted coding confidence</div>
      </div>
    </div>
  </div>

  <!-- github stats & trophy section with animation -->
  <div class="mt-5 text-center" data-aos="fade-up">
    <h2 class="fw-bold mb-3">📊 GitHub Analytics</h2>
    <div class="d-flex flex-wrap justify-content-center gap-4 align-items-center">
      <img src="https://github-readme-stats.vercel.app/api?username=Mainaky&show_icons=true&hide_border=true&title_color=1A56B0&icon_color=1A56B0&text_color=444444&bg_color=ffffff&count_private=true" height="170" alt="GitHub Stats" loading="lazy">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Mainaky&layout=compact&hide_border=true&title_color=1A56B0&text_color=444444&bg_color=ffffff" height="170" alt="Top Langs">
    </div>
    <div class="mt-3">
      <img src="https://streak-stats.demolab.com?user=Mainaky&hide_border=true&ring=1A56B0&fire=D14836&currStreakLabel=1A56B0&sideLabels=444444&dates=888888&background=ffffff" alt="GitHub Streak">
    </div>
    <div class="mt-4">
      <img src="https://github-profile-trophy.vercel.app/?username=Mainaky&theme=flat&no-frame=true&column=6&margin-w=8&margin-h=8" alt="trophy" width="100%">
    </div>
  </div>

  <!-- Relevant Coursework -->
  <div class="mt-5 p-4 stat-gradient rounded-4" data-aos="flip-up">
    <h3 class="fw-bold"><i class="fas fa-book-open"></i> 📚 Relevant Coursework</h3>
    <div class="d-flex flex-wrap gap-3 mt-3">
      <span class="badge-skill bg-white shadow-sm">Predictive Modeling for Data Science</span>
      <span class="badge-skill bg-white shadow-sm">Numerical Methods for Data Science</span>
      <span class="badge-skill bg-white shadow-sm">Inferential Statistics</span>
      <span class="badge-skill bg-white shadow-sm">Big Data Concepts</span>
      <span class="badge-skill bg-white shadow-sm">Artificial Intelligence</span>
      <span class="badge-skill bg-white shadow-sm">Object Oriented Programming</span>
    </div>
  </div>

  <!-- contact + footer CTA -->
  <div class="mt-5 text-center" data-aos="fade-up">
    <div class="glass-card p-5" style="background: linear-gradient(120deg, #ffffff, #f4f9ff);">
      <i class="fas fa-handshake fa-3x text-primary mb-3"></i>
      <h3 class="fw-bold">Let's Connect & Build Something Remarkable</h3>
      <p class="lead">Open to Internships | Research Collaborations | Open Source Contributions</p>
      <div class="d-flex flex-wrap justify-content-center gap-3 mt-3">
        <a href="https://www.linkedin.com/in/mainak-roy-7415b2258/" target="_blank" class="btn btn-primary rounded-pill px-4" style="background:#1A56B0; border:none;"><i class="fab fa-linkedin"></i> LinkedIn</a>
        <a href="mailto:mainak.roy23@st.niituniversity.in" class="btn btn-outline-primary rounded-pill px-4"><i class="fas fa-envelope"></i> Email Me</a>
        <a href="https://github.com/Mainaky" target="_blank" class="btn btn-dark rounded-pill px-4"><i class="fab fa-github"></i> GitHub Repos</a>
      </div>
    </div>
  </div>
</main>

<footer class="text-white text-center py-4 mt-5" style="background:#0b2b5c">
  <p class="mb-0 small">© 2026 Mainak Roy — Data Scientist | AI Engineer | MLOps Enthusiast</p>
  <p class="mb-0 small mt-1"><i class="fas fa-code"></i> Building intelligent systems that think & scale</p>
</footer>

<!-- Scripts for AOS -->
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
  AOS.init({
    duration: 800,
    once: true,
    offset: 20,
    easing: 'ease-out-quad'
  });
  // add additional interactive floating effect on skill cards? Already smooth
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if(entry.isIntersecting) entry.target.classList.add('float-animation');
    });
  }, { threshold: 0.3 });
  document.querySelectorAll('.project-card').forEach(card => observer.observe(card));
</script>
</body>
</html>
