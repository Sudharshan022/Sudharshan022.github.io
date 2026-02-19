# Sudharshan022.github.io[index.html.html](https://github.com/user-attachments/files/25417743/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>M Sudharshan</title>
  <meta name="description" content="M Sudharshan – AI & Data Science undergraduate, Python developer, web developer. Hyderabad, India." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />

  <style>
    /* ─── Reset ─────────────────────────────────────────────── */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { font-size: 16px; }
    body {
      font-family: 'Inter', sans-serif;
      background: #ffffff;
      color: #111111;
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }
    a { color: inherit; text-decoration: none; }
    ul { list-style: none; }

    /* ─── Layout ─────────────────────────────────────────────── */
    .container {
      max-width: 680px;
      margin: 0 auto;
      padding: 80px 24px 120px;
    }

    /* ─── Top Section ────────────────────────────────────────── */
    .profile {
      margin-bottom: 60px;
    }

    .profile-header {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 24px;
      margin-bottom: 24px;
    }

    .profile-info { flex: 1; }

    .profile-name {
      font-size: 2.2rem;
      font-weight: 700;
      letter-spacing: -0.03em;
      line-height: 1.1;
      margin-bottom: 6px;
    }

    .profile-location {
      font-size: 0.82rem;
      color: #888;
      display: flex;
      align-items: center;
      gap: 4px;
    }

    .profile-location::before {
      content: '📍';
      font-size: 0.75rem;
    }

    .profile-avatar {
      width: 72px;
      height: 72px;
      border-radius: 50%;
      background: #f0f0f0;
      border: 1px solid #e0e0e0;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.6rem;
      flex-shrink: 0;
      overflow: hidden;
    }

    .profile-bio {
      font-size: 0.95rem;
      font-weight: 500;
      color: #111;
      margin-bottom: 16px;
      line-height: 1.5;
    }

    .profile-bullets {
      display: flex;
      flex-direction: column;
      gap: 4px;
      margin-bottom: 28px;
    }

    .profile-bullets li {
      font-size: 0.88rem;
      color: #444;
      padding-left: 14px;
      position: relative;
    }

    .profile-bullets li::before {
      content: '-';
      position: absolute;
      left: 0;
      color: #999;
    }

    /* ─── Social Links ───────────────────────────────────────── */
    .socials {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }

    .social-link {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      font-size: 0.78rem;
      color: #555;
      border: 1px solid #e0e0e0;
      border-radius: 6px;
      padding: 5px 11px;
      transition: border-color 0.2s ease, color 0.2s ease;
    }

    .social-link:hover {
      border-color: #999;
      color: #111;
    }

    .social-link svg {
      width: 13px;
      height: 13px;
      fill: currentColor;
    }

    /* ─── Sections ───────────────────────────────────────────── */
    .section {
      margin-bottom: 52px;
    }

    .section-title {
      font-size: 1.05rem;
      font-weight: 600;
      letter-spacing: -0.01em;
      margin-bottom: 16px;
      color: #111;
    }

    /* ─── List Items ─────────────────────────────────────────── */
    .entry-list {
      display: flex;
      flex-direction: column;
    }

    .entry {
      display: flex;
      align-items: baseline;
      justify-content: space-between;
      gap: 12px;
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
      cursor: default;
    }

    .entry:last-child { border-bottom: none; }

    .entry-left {
      display: flex;
      align-items: center;
      gap: 10px;
      flex: 1;
      min-width: 0;
    }

    .entry-icon {
      width: 22px;
      height: 22px;
      border-radius: 5px;
      background: #f3f3f3;
      border: 1px solid #e8e8e8;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.7rem;
      flex-shrink: 0;
      overflow: hidden;
    }

    .entry-text {
      display: flex;
      flex-direction: column;
    }

    .entry-title {
      font-size: 0.88rem;
      font-weight: 400;
      color: #111;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      transition: color 0.15s ease;
    }

    .entry-sub {
      font-size: 0.76rem;
      color: #999;
      margin-top: 1px;
    }

    .entry-year {
      font-size: 0.82rem;
      color: #aaa;
      font-weight: 400;
      flex-shrink: 0;
      font-variant-numeric: tabular-nums;
    }

    /* ─── Giggle hover animation ─────────────────────────────── */
    @keyframes giggle {
      0%   { transform: translateX(0); }
      20%  { transform: translateX(-2px); }
      40%  { transform: translateX(2px); }
      60%  { transform: translateX(-1.5px); }
      80%  { transform: translateX(1.5px); }
      100% { transform: translateX(0); }
    }

    .entry:hover .entry-title {
      animation: giggle 0.35s ease;
      color: #000;
    }

    /* ─── Expandable details ─────────────────────────────────── */
    .entry-toggle {
      width: 18px;
      height: 18px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      cursor: pointer;
      color: #bbb;
      font-size: 0.7rem;
      transition: transform 0.2s ease, color 0.2s ease;
      user-select: none;
    }

    .entry.expanded .entry-toggle {
      transform: rotate(180deg);
      color: #555;
    }

    .entry-details {
      display: none;
      padding: 8px 0 10px 32px;
      font-size: 0.83rem;
      color: #666;
      line-height: 1.7;
      border-bottom: 1px solid #f0f0f0;
    }

    .entry-details.open { display: block; }

    .entry-details ul { display: flex; flex-direction: column; gap: 3px; }
    .entry-details li { padding-left: 12px; position: relative; }
    .entry-details li::before { content: '→'; position: absolute; left: 0; color: #bbb; font-size: 0.72rem; }

    /* ─── Footer ─────────────────────────────────────────────── */
    .footer {
      margin-top: 80px;
      padding-top: 24px;
      border-top: 1px solid #f0f0f0;
      font-size: 0.78rem;
      color: #bbb;
      text-align: center;
    }

    /* ─── Responsive ─────────────────────────────────────────── */
    @media (max-width: 520px) {
      .container { padding: 48px 20px 80px; }
      .profile-name { font-size: 1.8rem; }
      .profile-header { flex-direction: row; }
      .entry-title { font-size: 0.85rem; }
    }
  </style>
</head>
<body>

<div class="container">

  <!-- ── TOP SECTION ────────────────────────────────────────── -->
  <div class="profile">
    <div class="profile-header">
      <div class="profile-info">
        <h1 class="profile-name">M Sudharshan</h1>
        <p class="profile-location">Hyderabad, India</p>
      </div>
      <div class="profile-avatar"><img src="data:image/png;base64,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" alt="M Sudharshan" style="width:100%;height:100%;object-fit:cover;object-position:center top;" /></div>
    </div>

    <p class="profile-bio">
      I'm a final-year B.Tech AI & Data Science student, Python developer, and aspiring SDE from Hyderabad.
    </p>

    <ul class="profile-bullets">
      <li>Building Python-based apps and data pipelines using NumPy & Pandas</li>
      <li>Web development intern @ Prodigy Infotech — shipped real-world interfaces</li>
      <li>CGPA: 7.81 at Guru Nanak Institute of Technology</li>
      <li>Certified in Python (GeeksforGeeks) and TCS iON Career Edge</li>
      <li>Seeking internships & full-time SDE / ML Engineer roles</li>
    </ul>

    <div class="socials">
      <a href="/cdn-cgi/l/email-protection#a0cdc5c4c1d2c9d3d5c4c8c1d2d3c8c1cee0c7cdc1c9cc8ec3cfcd" class="social-link">
        <svg viewBox="0 0 24 24"><path d="M20 4H4a2 2 0 00-2 2v12a2 2 0 002 2h16a2 2 0 002-2V6a2 2 0 00-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
        Email
      </a>
      <a href="https://linkedin.com/in/sudharshanmahendra" class="social-link" target="_blank">
        <svg viewBox="0 0 24 24"><path d="M19 3H5a2 2 0 00-2 2v14a2 2 0 002 2h14a2 2 0 002-2V5a2 2 0 00-2-2zM9 17H7v-7h2v7zm-1-8a1 1 0 110-2 1 1 0 010 2zm9 8h-2v-3.5c0-1-.8-1.5-1.5-1.5s-1.5.5-1.5 1.5V17h-2v-7h2v1c.5-.8 1.4-1 2-1 1.9 0 3 1.3 3 3.3V17z"/></svg>
        LinkedIn
      </a>
      <a href="https://github.com/Sudharshan022" class="social-link" target="_blank">
        <svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.58 2 12.26c0 4.54 2.87 8.39 6.84 9.75.5.09.68-.22.68-.49v-1.71c-2.78.62-3.37-1.37-3.37-1.37-.45-1.18-1.11-1.5-1.11-1.5-.91-.64.07-.62.07-.62 1 .07 1.53 1.06 1.53 1.06.89 1.57 2.34 1.12 2.91.85.09-.66.35-1.12.63-1.38-2.22-.26-4.56-1.14-4.56-5.07 0-1.12.39-2.03 1.03-2.75-.1-.26-.45-1.3.1-2.71 0 0 .84-.28 2.75 1.05A9.36 9.36 0 0112 7.43c.85 0 1.71.12 2.51.34 1.91-1.33 2.75-1.05 2.75-1.05.55 1.41.2 2.45.1 2.71.64.72 1.03 1.63 1.03 2.75 0 3.94-2.34 4.81-4.57 5.06.36.32.68.94.68 1.9v2.82c0 .27.18.59.69.49A10.27 10.27 0 0022 12.26C22 6.58 17.52 2 12 2z"/></svg>
        GitHub
      </a>
      <a href="tel:+916281251023" class="social-link">
        <svg viewBox="0 0 24 24"><path d="M6.6 10.8c1.4 2.8 3.8 5.1 6.6 6.6l2.2-2.2c.3-.3.7-.4 1-.2 1.1.4 2.3.6 3.6.6.6 0 1 .4 1 1V20c0 .6-.4 1-1 1C10.6 21 3 13.4 3 4c0-.6.4-1 1-1h3.5c.6 0 1 .4 1 1 0 1.3.2 2.5.6 3.6.1.3 0 .7-.2 1L6.6 10.8z"/></svg>
        +91 6281251023
      </a>
    </div>
  </div>

  <!-- ── SOFTWARE / PROJECTS ─────────────────────────────────── -->
  <div class="section">
    <h2 class="section-title">Software</h2>
    <ul class="entry-list">

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🖥️</div>
          <div class="entry-text">
            <span class="entry-title">Interactive Landing Page</span>
            <span class="entry-sub">HTML · CSS · JavaScript</span>
          </div>
        </div>
        <span class="entry-year">2024</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        <ul>
          <li>Dynamic sticky navigation menu that changes style on scroll and hover</li>
          <li>Fully responsive across desktop, tablet, and mobile</li>
          <li>Smooth CSS transitions and hover animations throughout</li>
        </ul>
      </li>

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">⏱️</div>
          <div class="entry-text">
            <span class="entry-title">Stopwatch Web Application</span>
            <span class="entry-sub">HTML · CSS · JavaScript</span>
          </div>
        </div>
        <span class="entry-year">2024</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        <ul>
          <li>Start, pause, and reset functionality with precise timing logic</li>
          <li>Lap tracking — records and displays multiple lap timestamps</li>
          <li>Zero dependencies, pure JavaScript, instant load</li>
        </ul>
      </li>

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">📊</div>
          <div class="entry-text">
            <span class="entry-title">ML Data Analysis Notebooks</span>
            <span class="entry-sub">Python · NumPy · Pandas · Scikit-learn</span>
          </div>
        </div>
        <span class="entry-year">2024</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        <ul>
          <li>EDA pipelines with data cleaning, transformation, and visual storytelling</li>
          <li>Classification and regression experiments with model evaluation</li>
          <li>Confusion matrices, accuracy metrics, and feature analysis</li>
        </ul>
      </li>

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🐍</div>
          <div class="entry-text">
            <span class="entry-title">Python Automation Toolkit</span>
            <span class="entry-sub">Python · Django · MySQL</span>
          </div>
        </div>
        <span class="entry-year">2023</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        <ul>
          <li>Batch file management and data processing scripts</li>
          <li>Web scraping utilities for structured data collection</li>
          <li>Django-backed mini CRUD application with MySQL</li>
        </ul>
      </li>

    </ul>
  </div>

  <!-- ── CERTIFICATIONS / AWARDS ─────────────────────────────── -->
  <div class="section">
    <h2 class="section-title">Awards &amp; Certifications</h2>
    <ul class="entry-list">

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🐍</div>
          <div class="entry-text">
            <span class="entry-title">Python Programming Certification</span>
            <span class="entry-sub">GeeksforGeeks Nation Skillup</span>
          </div>
        </div>
        <span class="entry-year">2025</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        Verified certification covering Python fundamentals, data structures, OOP, and file handling through GeeksforGeeks' national skills assessment platform.
      </li>

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🏆</div>
          <div class="entry-text">
            <span class="entry-title">TCS iON Career Edge – Young Professional</span>
            <span class="entry-sub">Tata Consultancy Services</span>
          </div>
        </div>
        <span class="entry-year">2025</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        Industry-recognized program covering professional skills, business communication, aptitude, and technical readiness for entering the IT workforce.
      </li>

    </ul>
  </div>

  <!-- ── WORK ───────────────────────────────────────────────── -->
  <div class="section">
    <h2 class="section-title">Work</h2>
    <ul class="entry-list">

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">💻</div>
          <div class="entry-text">
            <span class="entry-title">Web Development Intern @ Prodigy Infotech</span>
            <span class="entry-sub">HTML · CSS · JavaScript · Git</span>
          </div>
        </div>
        <span class="entry-year">2024</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        <ul>
          <li>Built and shipped responsive web interfaces served to live users</li>
          <li>Followed professional code review and version control workflows</li>
          <li>Debugged cross-browser issues and improved page load performance</li>
          <li>Delivered all projects on schedule within team deadlines</li>
        </ul>
      </li>

    </ul>
  </div>

  <!-- ── EDUCATION ──────────────────────────────────────────── -->
  <div class="section">
    <h2 class="section-title">Education</h2>
    <ul class="entry-list">

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🎓</div>
          <div class="entry-text">
            <span class="entry-title">B.Tech – AI & Data Science @ GNIT Hyderabad</span>
            <span class="entry-sub">CGPA: 7.81 / 10</span>
          </div>
        </div>
        <span class="entry-year">2023 – 2026</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        Guru Nanak Institute of Technology, Hyderabad. Coursework: Machine Learning, Data Structures, Database Management, Python Programming, Web Technologies, Deep Learning, Statistics for AI.
      </li>

      <li class="entry" onclick="toggleEntry(this)">
        <div class="entry-left">
          <div class="entry-icon">🏫</div>
          <div class="entry-text">
            <span class="entry-title">Diploma – Electrical & Electronics Engineering</span>
            <span class="entry-sub">Government Polytechnic College, Mahabubnagar · CGPA: 7.07</span>
          </div>
        </div>
        <span class="entry-year">2022</span>
        <span class="entry-toggle">▾</span>
      </li>
      <li class="entry-details">
        Built foundations in analytical thinking, circuit analysis, and technical problem solving — the roots of my engineering mindset.
      </li>

    </ul>
  </div>

  <!-- ── FOOTER ─────────────────────────────────────────────── -->
  <div class="footer">
    M Sudharshan · Hyderabad, India · <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="7518101114071c0600111d1407061d141b351218141c195b161a18">[email&#160;protected]</a>
  </div>

</div>

<script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>
  function toggleEntry(e
