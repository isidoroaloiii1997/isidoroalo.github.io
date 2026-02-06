<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Isidoro Alo III | Remote Professional Portfolio</title>

  <!-- MOBILE-FIRST STYLE -->
  <style>
    :root {
      --dark:#0f172a;
      --mid:#1e293b;
      --light:#f8fafc;
      --accent:#2563eb;
    }

    * { box-sizing:border-box; }
    body { margin:0; font-family:Arial, sans-serif; background:var(--light); color:#333; }

    header { background:var(--dark); color:#fff; padding:32px 16px; text-align:center; }
    header h1 { margin:0; font-size:1.8rem; }
    header p { margin:8px 0 16px; }

    .cta a {
      display:inline-block; padding:10px 16px; margin:4px;
      background:var(--accent); color:#fff; text-decoration:none; border-radius:6px;
      font-weight:bold; font-size:0.9rem;
    }

    nav { background:var(--mid); display:flex; justify-content:center; flex-wrap:wrap; }
    nav button {
      background:none; border:none; color:#fff; padding:12px 14px; cursor:pointer;
      font-weight:bold; font-size:0.9rem;
    }
    nav button.active { border-bottom:2px solid var(--accent); }

    section { display:none; padding:24px 16px; max-width:1100px; margin:auto; }
    section.active { display:block; }

    h2 { color:var(--dark); margin-top:0; border-bottom:2px solid #e5e7eb; padding-bottom:6px; }

    .grid { display:grid; grid-template-columns:1fr; gap:16px; }
    .card { background:#fff; padding:16px; border-radius:8px; box-shadow:0 2px 4px rgba(0,0,0,0.05); }

    footer { text-align:center; padding:20px; background:var(--dark); color:#fff; }

    /* DESKTOP VIEW */
    @media (min-width: 768px) {
      header h1 { font-size:2.4rem; }
      .grid { grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); }
    }
  </style>

  <script>
    function showTab(id) {
      document.querySelectorAll('section').forEach(s => s.classList.remove('active'));
      document.querySelectorAll('nav button').forEach(b => b.classList.remove('active'));
      document.getElementById(id).classList.add('active');
      document.getElementById('btn-' + id).classList.add('active');
    }
    window.onload = () => showTab('about');
  </script>
</head>
<body>

<header>
  <h1>Isidoro D. Alo III</h1>
  <p>Virtual Assistant | Estimator | AutoCAD Professional | Financial & Insurance Consultant</p>

  <div class="cta">
    <a href="CV-Isidoro-Alo.pdf" download>Download CV</a>
    <a href="#contact" onclick="showTab('contact')">Hire Me</a>
  </div>
</header>

<nav>
  <button id="btn-about" onclick="showTab('about')">About</button>
  <button id="btn-va" onclick="showTab('va')">VA</button>
  <button id="btn-engineer" onclick="showTab('engineer')">Engineer</button>
  <button id="btn-finance" onclick="showTab('finance')">Finance</button>
  <button id="btn-contact" onclick="showTab('contact')">Contact</button>
</nav>

<section id="about">
  <h2>About Me</h2>
  <p>I am a results-driven remote professional with experience in engineering, estimation, AutoCAD drafting, virtual assistance, and financial consulting. I help businesses stay organized, efficient, and profitable through structured support and technical expertise.</p>
</section>

<section id="va">
  <h2>Virtual Assistant Services</h2>
  <div class="grid">
    <div class="card">Email & Calendar Management</div>
    <div class="card">Project Tracking & Reports</div>
    <div class="card">Client Communication & Follow‑ups</div>
    <div class="card">Documentation & Admin Support</div>
  </div>
</section>

<section id="engineer">
  <h2>Engineering & AutoCAD Services</h2>
  <div class="grid">
    <div class="card">Cost Estimation & Quantity Take‑Offs</div>
    <div class="card">2D AutoCAD Drafting & Revisions</div>
    <div class="card">Technical Documentation</div>
    <div class="card">Project Coordination & QA</div>
  </div>
</section>

<section id="finance">
  <h2>Financial & Insurance Consulting</h2>
  <div class="grid">
    <div class="card">Financial Planning & Goal Setting</div>
    <div class="card">Life & Health Insurance Advisory</div>
    <div class="card">Client Presentations & Training</div>
    <div class="card">Long‑term Wealth Strategies</div>
  </div>
</section>

<section id="contact">
  <h2>Contact Information</h2>
  <div class="grid">
    <div class="card">📞 +63 920 359 2491</div>
    <div class="card">📧 isidoroaloiii1997@gmail.com</div>
    <div class="card"><a href="https://www.linkedin.com/in/isidoro-iii-alo-251998385" target="_blank">LinkedIn Profile</a></div>
    <div class="card"><a href="https://www.facebook.com/isidoro.alo/" target="_blank">Facebook</a></div>
    <div class="card"><a href="https://www.onlinejobs.ph/jobseekers/info/3069284" target="_blank">OnlineJobs.ph</a></div>
  </div>
</section>

<footer>
  © 2026 Isidoro D. Alo III | Remote Professional Portfolio
</footer>

</body>
</html>
