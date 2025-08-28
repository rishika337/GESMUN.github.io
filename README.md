# GESMUN.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>[Your School] MUN — 31 Oct & 1 Nov</title>
  <meta name="description" content="Official website for the internal [Your School] Model United Nations (MUN) to be held on 31 October & 1 November." />
  <meta name="theme-color" content="#0f172a" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />
  <style>
    :root{
      --bg: #0b1020;        /* page background */
      --card:#0f172a;       /* card background */
      --muted:#cbd5e1;      /* muted text */
      --text:#e2e8f0;       /* main text */
      --accent:#60a5fa;     /* accent */
      --accent-2:#22d3ee;   /* secondary accent */
      --ring: 0 10px 40px rgba(32,84,209,.25);
      --radius: 16px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,"Helvetica Neue",Arial,"Noto Sans",sans-serif;background:linear-gradient(180deg,#0b1020 0%,#0b1020 30%,#0c1226 100%);color:var(--text);} 
    a{color:inherit;text-decoration:none}
    .container{max-width:1080px;margin-inline:auto;padding:24px}
    .btn{display:inline-flex;align-items:center;gap:.6rem;padding:.9rem 1.2rem;border-radius:999px;background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#001018;font-weight:700;box-shadow:var(--ring);transition:transform .15s ease,filter .15s ease}
    .btn:hover{transform:translateY(-2px);filter:brightness(1.05)}
    .btn.secondary{background:#111826;color:var(--text);border:1px solid #22314f;box-shadow:none}
    header{position:sticky;top:0;backdrop-filter:saturate(180%) blur(10px);background:rgba(3,8,23,.6);border-bottom:1px solid rgba(148,163,184,.12);z-index:20}
    .nav{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:.8rem}
    .brand-logo{width:40px;height:40px;border-radius:10px;background:radial-gradient(120% 120% at 20% 0%,#60a5fa,#22d3ee);box-shadow:0 8px 30px rgba(34,211,238,.35)}
    .brand h1{font-size:1.05rem;margin:0;font-weight:800;letter-spacing:.2px}
    .nav-links{display:flex;gap:1.1rem;align-items:center}
    .nav-links a{color:var(--muted);font-weight:600}
    .nav-links a:hover{color:#fff}
    .mobile-toggle{display:none}

    .hero{display:grid;grid-template-columns:1.2fr .8fr;gap:26px;align-items:center;padding:40px 0}
    .card{background:linear-gradient(180deg,rgba(255,255,255,.03),rgba(255,255,255,.02));border:1px solid rgba(148,163,184,.12);border-radius:var(--radius);padding:24px;box-shadow:0 12px 60px rgba(0,0,0,.25)}
    .pill{display:inline-flex;align-items:center;gap:.5rem;border:1px solid rgba(148,163,184,.2);border-radius:999px;padding:.35rem .7rem;color:var(--muted);font-weight:600}
    .title{font-size:clamp(28px,4.2vw,54px);line-height:1.05;margin:16px 0 10px;font-weight:800}
    .subtitle{font-size:clamp(14px,1.5vw,18px);color:var(--muted);margin:0 0 22px}
    .kpis{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
    .kpi{padding:14px;border-radius:12px;background:#0c162b;border:1px solid rgba(148,163,184,.15);text-align:center}
    .kpi strong{display:block;font-size:1.2rem}

    .countdown{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-top:16px}
    .tile{padding:16px 10px;text-align:center;border:1px solid rgba(148,163,184,.15);background:#0b162c;border-radius:12px}
    .tile span{display:block}
    .lg{font-size:1.6rem;font-weight:800}
    .sm{font-size:.8rem;color:var(--muted);letter-spacing:.4px}

    section{padding:34px 0}
    h2{margin:0 0 14px;font-size:1.6rem}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}

    .committee{display:flex;flex-direction:column;gap:10px}
    .committee h3{margin:0;font-size:1.1rem}
    .committee .meta{font-size:.9rem;color:var(--muted)}

    .schedule table{width:100%;border-collapse:collapse}
    .schedule th,.schedule td{border-bottom:1px dashed rgba(148,163,184,.2);padding:10px;text-align:left}
    .schedule th{color:#cbd5e1;font-weight:700}

    .faq details{background:#0e182e;border:1px solid rgba(148,163,184,.15);border-radius:12px;padding:14px}
    .faq details+details{margin-top:10px}
    .faq summary{cursor:pointer;font-weight:700}

    .footer{padding:30px 0;color:#a8b1c5;border-top:1px solid rgba(148,163,184,.12)}
    .footer small{display:block;margin-top:6px}

    /* responsiveness */
    @media (max-width: 880px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr;}
      .nav-links{display:none}
      .mobile-toggle{display:inline-flex;border:1px solid rgba(148,163,184,.2);border-radius:999px;padding:.5rem .7rem;color:var(--muted);font-weight:700}
      .countdown{grid-template-columns:repeat(2,1fr)}
    }
  </style>
</head>
<body>
  <!-- ================= NAVBAR ================= -->
  <header>
    <div class="container nav">
      <a class="brand" href="#home" aria-label="Go to top">
        <div class="brand-logo" aria-hidden="true"></div>
        <h1 id="home">[Your School] MUN</h1>
      </a>
      <nav class="nav-links" aria-label="primary">
        <a href="#about">About</a>
        <a href="#committees">Committees</a>
        <a href="#schedule">Schedule</a>
        <a href="#resources">Resources</a>
        <a href="#contact">Contact</a>
        <a class="btn" href="#register">Register</a>
      </nav>
      <button class="mobile-toggle" aria-label="Open menu" onclick="document.querySelector('.drawer').showModal()">Menu</button>
    </div>
  </header>

  <!-- mobile menu -->
  <dialog class="drawer" style="background:#0b1226;border:1px solid rgba(148,163,184,.2);border-radius:12px;padding:18px;max-width:520px;width:90%">
    <form method="dialog">
      <h3 style="margin-top:0">Menu</h3>
      <p><a href="#about">About</a></p>
      <p><a href="#committees">Committees</a></p>
      <p><a href="#schedule">Schedule</a></p>
      <p><a href="#resources">Resources</a></p>
      <p><a href="#contact">Contact</a></p>
      <p><a class="btn" href="#register">Register</a></p>
      <div style="text-align:right;margin-top:10px"><button class="btn secondary">Close</button></div>
    </form>
  </dialog>

  <!-- ================= HERO ================= -->
  <div class="container hero">
    <div class="card">
      <span class="pill">Internal Conference · On Campus</span>
      <h2 class="title">[Your School] Model United Nations</h2>
      <p class="subtitle">Join us for a two‑day debate and diplomacy experience on <strong>31 October</strong> & <strong>1 November</strong>. Open to students from classes <strong>VIII–XII</strong>. No prior MUN experience required!</p>
      <div class="kpis">
        <div class="kpi"><strong>2</strong><span class="sm">Days</span></div>
        <div class="kpi"><strong>4+</strong><span class="sm">Committees</span></div>
        <div class="kpi"><strong>Best Delegate</strong><span class="sm">Awards</span></div>
      </div>
      <div class="countdown" id="countdown" aria-live="polite"></div>
      <div style="display:flex;gap:10px;margin-top:16px;flex-wrap:wrap">
        <a class="btn" href="#register">Register Now</a>
        <a class="btn secondary" href="#resources">View Resources</a>
      </div>
    </div>
    <div class="card" style="background:radial-gradient(100% 120% at 0% 0%, rgba(34,211,238,.2), transparent 40%), linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));display:grid;place-items:center;min-height:280px">
      <div style="text-align:center;max-width:420px">
        <img alt="MUN Illustration" src="https://images.unsplash.com/photo-1542038784456-1ea8e935640e?q=80&w=1000&auto=format&fit=crop" style="width:100%;height:auto;border-radius:12px;border:1px solid rgba(148,163,184,.2)"/>
        <p class="sm" style="margin-top:10px">Photo courtesy of Unsplash — replace with your school photo or logo.</p>
      </div>
    </div>
  </div>

  <!-- ================= ABOUT ================= -->
  <section id="about">
    <div class="container">
      <div class="card">
        <h2>About the Conference</h2>
        <p>Our internal Model United Nations fosters public speaking, research, negotiation, and teamwork. Delegates will represent countries, draft resolutions, and collaborate to address global challenges in a respectful, academic setting.</p>
        <p><strong>Venue:</strong> [Your School Name], [City]. <strong>Dates:</strong> 31 October & 1 November, <span id="year-label">[Year]</span>.</p>
      </div>
    </div>
  </section>

  <!-- ================= COMMITTEES ================= -->
  <section id="committees">
    <div class="container">
      <h2>Committees & Agendas</h2>
      <div class="grid">
        <div class="card committee">
          <h3>UN General Assembly (DISEC)</h3>
          <div class="meta">Agenda: Strengthening global frameworks against cyber warfare.</div>
          <div class="meta">Bureau: Chair, Vice‑Chair, Rapporteur</div>
          <a class="btn secondary" href="#register">Apply as Delegate</a>
        </div>
        <div class="card committee">
          <h3>UN Security Council</h3>
          <div class="meta">Agenda: Situation in the [Region] — immediate measures for ceasefire.</div>
          <div class="meta">Bureau: President, Vice‑President</div>
          <a class="btn secondary" href="#register">Apply as Delegate</a>
        </div>
        <div class="card committee">
          <h3>WHO</h3>
          <div class="meta">Agenda: Coordinated responses to emerging zoonotic diseases.</div>
          <div class="meta">Bureau: Chair, Vice‑Chair</div>
          <a class="btn secondary" href="#register">Apply as Delegate</a>
        </div>
        <div class="card committee">
          <h3>UNESCO</h3>
          <div class="meta">Agenda: Equitable access to digital education resources.</div>
          <div class="meta">Bureau: Chair, Vice‑Chair</div>
          <a class="btn secondary" href="#register">Apply as Delegate</a>
        </div>
        <div class="card committee">
          <h3>Press Corps (IPC)</h3>
          <div class="meta">Agenda: Live coverage and press conferences across committees.</div>
          <div class="meta">Bureau: Editor‑in‑Chief</div>
          <a class="btn secondary" href="#register">Apply as Journalist</a>
        </div>
        <div class="card committee">
          <h3>Executive Board</h3>
          <div class="meta">Applications for Chairs/Co‑Chairs for experienced MUNners.</div>
          <a class="btn secondary" href="#register">Apply for EB</a>
        </div>
      </div>
    </div>
  </section>

  <!-- ================= SCHEDULE ================= -->
  <section id="schedule" class="schedule">
    <div class="container">
      <h2>Conference Schedule</h2>
      <div class="card">
        <h3>Day 1 — 31 October</h3>
        <table aria-label="Day 1 schedule">
          <thead><tr><th>Time</th><th>Activity</th><th>Location</th></tr></thead>
          <tbody>
            <tr><td>08:00 – 09:00</td><td>Registration & Allotments</td><td>School Auditorium</td></tr>
            <tr><td>09:00 – 09:45</td><td>Opening Ceremony</td><td>Auditorium</td></tr>
            <tr><td>10:00 – 13:00</td><td>Committee Session I</td><td>Respective Rooms</td></tr>
            <tr><td>13:00 – 14:00</td><td>Lunch</td><td>Cafeteria</td></tr>
            <tr><td>14:00 – 16:30</td><td>Committee Session II</td><td>Respective Rooms</td></tr>
          </tbody>
        </table>
      </div>
      <div class="card" style="margin-top:12px">
        <h3>Day 2 — 1 November</h3>
        <table aria-label="Day 2 schedule">
          <thead><tr><th>Time</th><th>Activity</th><th>Location</th></tr></thead>
          <tbody>
            <tr><td>08:30 – 10:45</td><td>Committee Session III</td><td>Respective Rooms</td></tr>
            <tr><td>11:00 – 12:30</td><td>Press Conferences</td><td>Auditorium</td></tr>
            <tr><td>12:30 – 13:30</td><td>Lunch</td><td>Cafeteria</td></tr>
            <tr><td>13:30 – 15:30</td><td>Committee Session IV</td><td>Respective Rooms</td></tr>
            <tr><td>16:00 – 17:00</td><td>Closing & Awards</td><td>Auditorium</td></tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>

  <!-- ================= RESOURCES ================= -->
  <section id="resources">
    <div class="container">
      <h2>Resources</h2>
      <div class="grid">
        <div class="card">
          <h3>Background Guides</h3>
          <p>Download background guides for each committee. (Replace links below.)</p>
          <ul>
            <li><a href="#">DISEC BG (PDF)</a></li>
            <li><a href="#">UNSC BG (PDF)</a></li>
            <li><a href="#">WHO BG (PDF)</a></li>
            <li><a href="#">UNESCO BG (PDF)</a></li>
          </ul>
        </div>
        <div class="card">
          <h3>Rules of Procedure</h3>
          <p>Our ROP is a simplified hybrid of UN protocols, ideal for first‑time delegates.</p>
          <p><a class="btn secondary" href="#">Download ROP (PDF)</a></p>
        </div>
        <div class="card">
          <h3>Position Paper Template</h3>
          <p>Use this template to structure your research and country stance.</p>
          <p><a class="btn secondary" href="#">Download DOCX</a></p>
        </div>
      </div>
    </div>
  </section>

  <!-- ================= REGISTRATION ================= -->
  <section id="register">
    <div class="container">
      <div class="card">
        <h2>Registration</h2>
        <p>Spots are limited. Submit the form below to apply as a delegate, journalist, or EB member. You’ll receive allotments by email.</p>
        <!-- Replace the iframe src with your Google Form link -->
        <iframe title="Registration Form" src="https://docs.google.com/forms/d/e/1FAIpQLSf-demo-form/viewform?embedded=true" width="100%" height="720" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
        <p class="sm" style="margin-top:10px">Don’t have Google Forms? Replace the iframe with a <a href="mailto:mun@your-school.edu">mailto</a> link or any other form service.</p>
      </div>
    </div>
  </section>

  <!-- ================= CONTACT ================= -->
  <section id="contact">
    <div class="container">
      <div class="card">
        <h2>Contact</h2>
        <p>Have questions? Reach us at <a href="mailto:mun@your-school.edu">mun@your-school.edu</a> or visit the Student Council room during recess.</p>
        <div class="grid">
          <div>
            <h3>Secretariat</h3>
            <ul>
              <li>Secretary‑General — [Name]</li>
              <li>Director‑General — [Name]</li>
              <li>USG Academics — [Name]</li>
            </ul>
          </div>
          <div>
            <h3>Venue</h3>
            <p>[Your School Name], [Street Address], [City]</p>
            <p><a class="btn secondary" href="https://maps.google.com" target="_blank" rel="noopener">Open in Maps</a></p>
          </div>
          <div>
            <h3>Social</h3>
            <p><a href="#">Instagram</a> · <a href="#">YouTube</a></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="container">
      <div style="display:flex;justify-content:space-between;gap:10px;flex-wrap:wrap">
        <div>
          <strong>[Your School] MUN</strong>
          <small>© <span id="year">2025</span> — For educational use</small>
        </div>
        <div>
          <small>Built with ♥ — <a href="https://github.com">GitHub Pages</a></small>
        </div>
      </div>
    </div>
  </footer>

  <script>
    // ======== QUICK SETTINGS (edit these!) ========
    const SCHOOL_NAME = "[Your School]";          // shown in title & headings
    const YEAR = new Date().getFullYear();        // set to a specific year if needed
    const EVENT_TZ = "Asia/Kolkata";              // timezone for countdown

    // If your event is NEXT YEAR, set YEAR manually above.
    // Dates: 31 Oct & 1 Nov of YEAR

    document.title = `${SCHOOL_NAME} MUN — 31 Oct & 1 Nov`;
    document.querySelector('h1').textContent = `${SCHOOL_NAME} MUN`;
    document.getElementById('year').textContent = YEAR;
    document.getElement
