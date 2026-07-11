<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Yuvaraaj R K — Software Developer</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');

  :root{
    --ink:#12151c;
    --panel:#1a1f2b;
    --paper:#eeeee6;
    --amber:#e8b84b;
    --amber-dim:#a9863c;
    --line: rgba(238,238,230,0.14);
    --muted:#9aa0ad;
  }

  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--ink);
    color:var(--paper);
    font-family:'Inter',sans-serif;
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
  }

  a{color:var(--amber);text-decoration:none;border-bottom:1px solid transparent;}
  a:hover{border-bottom-color:var(--amber);}

  .wrap{
    max-width:860px;
    margin:0 auto;
    padding:64px 40px 80px;
  }

  /* ---------- HERO / TERMINAL HEADER ---------- */
  .term{
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:10px;
    overflow:hidden;
    margin-bottom:48px;
  }
  .term-bar{
    display:flex;
    align-items:center;
    gap:8px;
    padding:11px 16px;
    background:#151923;
    border-bottom:1px solid var(--line);
  }
  .dot{width:10px;height:10px;border-radius:50%;}
  .dot.r{background:#e0605a;}
  .dot.y{background:#e8b84b;}
  .dot.g{background:#59c27c;}
  .term-title{
    margin-left:8px;
    font-family:'JetBrains Mono',monospace;
    font-size:12px;
    color:var(--muted);
  }
  .term-body{padding:28px 32px 34px;}
  .prompt{
    font-family:'JetBrains Mono',monospace;
    font-size:13px;
    color:var(--amber);
    margin:0 0 6px;
  }
  .prompt span{color:var(--muted);}
  h1{
    font-family:'Space Grotesk',sans-serif;
    font-size:44px;
    font-weight:700;
    letter-spacing:-0.01em;
    margin:4px 0 6px;
    color:var(--paper);
  }
  .role{
    font-family:'Space Grotesk',sans-serif;
    font-size:16px;
    font-weight:500;
    color:var(--amber);
    margin:0 0 20px;
  }
  .contact-row{
    display:flex;
    flex-wrap:wrap;
    gap:6px 22px;
    font-family:'JetBrains Mono',monospace;
    font-size:12.5px;
    color:var(--muted);
  }
  .contact-row a{color:var(--muted);}
  .contact-row a:hover{color:var(--amber);border-bottom-color:var(--amber);}
  .contact-row .k{color:var(--amber-dim);}

  /* ---------- SECTIONS ---------- */
  section{margin-bottom:38px;}
  .sec-head{
    display:flex;
    align-items:baseline;
    gap:10px;
    margin-bottom:18px;
  }
  .sec-tag{
    font-family:'JetBrains Mono',monospace;
    font-size:12px;
    color:var(--amber-dim);
  }
  .sec-head h2{
    font-family:'Space Grotesk',sans-serif;
    font-size:13px;
    font-weight:600;
    text-transform:uppercase;
    letter-spacing:0.12em;
    color:var(--paper);
    margin:0;
    white-space:nowrap;
  }
  .sec-head .rule{
    flex:1;
    height:1px;
    background:var(--line);
  }

  /* Objective */
  .objective{
    font-size:15px;
    color:#cfd3da;
    max-width:70ch;
    border-left:2px solid var(--amber-dim);
    padding-left:18px;
  }

  /* Education */
  .edu-row{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;
    gap:16px;
    flex-wrap:wrap;
  }
  .edu-name{
    font-family:'Space Grotesk',sans-serif;
    font-weight:600;
    font-size:16px;
    color:var(--paper);
  }
  .edu-sub{font-size:13.5px;color:var(--muted);margin-top:3px;}
  .edu-meta{
    text-align:right;
    font-family:'JetBrains Mono',monospace;
    font-size:12.5px;
    color:var(--amber);
    white-space:nowrap;
  }
  .edu-meta .cgpa{display:block;color:var(--muted);margin-top:3px;}

  /* Projects / Experience cards */
  .card{
    padding:18px 20px;
    border:1px solid var(--line);
    border-radius:8px;
    background:linear-gradient(180deg, rgba(255,255,255,0.015), transparent);
    margin-bottom:14px;
  }
  .card-head{
    display:flex;
    justify-content:space-between;
    align-items:baseline;
    gap:12px;
    flex-wrap:wrap;
    margin-bottom:8px;
  }
  .card-title{
    font-family:'Space Grotesk',sans-serif;
    font-weight:600;
    font-size:15.5px;
    color:var(--paper);
  }
  .card-date{
    font-family:'JetBrains Mono',monospace;
    font-size:11.5px;
    color:var(--amber-dim);
    white-space:nowrap;
  }
  .card ul{
    margin:0;
    padding-left:18px;
    font-size:14px;
    color:#c6cad2;
  }
  .card ul li{margin-bottom:4px;}
  .card ul li::marker{color:var(--amber-dim);}

  /* Skills */
  .skill-grid{
    display:grid;
    grid-template-columns:140px 1fr;
    row-gap:12px;
    column-gap:16px;
    font-size:13.5px;
  }
  .skill-cat{
    font-family:'JetBrains Mono',monospace;
    color:var(--amber-dim);
    font-size:12px;
    padding-top:3px;
  }
  .tag-row{display:flex;flex-wrap:wrap;gap:8px;}
  .tag{
    font-family:'JetBrains Mono',monospace;
    font-size:12px;
    padding:4px 10px;
    border:1px solid var(--line);
    border-radius:5px;
    color:#dcdfe5;
    background:rgba(255,255,255,0.02);
  }

  /* Certifications / Achievements */
  .plain-list{list-style:none;margin:0;padding:0;}
  .plain-list li{
    display:flex;
    justify-content:space-between;
    gap:12px;
    padding:9px 0;
    border-bottom:1px solid var(--line);
    font-size:14px;
    color:#cfd3da;
  }
  .plain-list li:last-child{border-bottom:none;}
  .plain-list .when{
    font-family:'JetBrains Mono',monospace;
    font-size:11.5px;
    color:var(--muted);
    white-space:nowrap;
  }

  /* Soft skills */
  .soft-row{display:flex;flex-wrap:wrap;gap:10px;}
  .soft{
    font-size:13px;
    padding:6px 14px;
    border-radius:20px;
    border:1px solid var(--amber-dim);
    color:var(--amber);
  }

  footer{
    margin-top:50px;
    text-align:center;
    font-family:'JetBrains Mono',monospace;
    font-size:11px;
    color:var(--muted);
  }

  @media (max-width:600px){
    .wrap{padding:36px 18px 60px;}
    h1{font-size:32px;}
    .term-body{padding:22px 18px 26px;}
    .skill-grid{grid-template-columns:1fr;}
    .edu-meta{text-align:left;}
  }

  @media print{
    body{background:#fff;color:#111;}
    .wrap{max-width:100%;padding:20px 28px;}
    .term{background:#fff;border-color:#ccc;}
    .term-bar{background:#f4f4f4;}
    h1,.card-title,.edu-name,.sec-head h2{color:#111;}
    .role{color:#8a6a1f;}
    .card{background:none;border-color:#ddd;}
    .prompt,.contact-row,.contact-row a{color:#555;}
    a{color:#8a6a1f;}
  }
</style>
</head>
<body>
<div class="wrap">

  <div class="term">
    <div class="term-bar">
      <div class="dot r"></div><div class="dot y"></div><div class="dot g"></div>
      <div class="term-title">resume.sh — yuvaraaj-r-k</div>
    </div>
    <div class="term-body">
      <p class="prompt"><span>$</span> whoami</p>
      <h1>Yuvaraaj R K</h1>
      <p class="role">Software Developer · Full-Stack &amp; AI-Integrated Systems</p>
      <div class="contact-row">
        <span><span class="k">loc</span> Salem, Tamil Nadu</span>
        <span><span class="k">tel</span> +91 9994883043</span>
        <span><span class="k">mail</span> <a href="mailto:yuvarajamanikkam@gmail.com">yuvarajamanikkam@gmail.com</a></span>
        <span><span class="k">git</span> <a href="https://github.com/yuvaraaj-29" target="_blank">github.com/yuvaraaj-29</a></span>
        <span><span class="k">in</span> <a href="https://linkedin.com/in/yuvaraaj-r-k-556599357" target="_blank">linkedin.com/in/yuvaraaj-r-k</a></span>
      </div>
    </div>
  </div>

  <section>
    <div class="sec-head"><span class="sec-tag">01</span><h2>Objective</h2><div class="rule"></div></div>
    <p class="objective">Aspiring Software Developer with strong knowledge in Java, Python, and full-stack development. Passionate about building scalable applications, automation systems, and AI-powered software solutions — seeking to contribute to real-world development work at a technology-driven organization.</p>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">02</span><h2>Education</h2><div class="rule"></div></div>
    <div class="edu-row">
      <div>
        <div class="edu-name">Mepco Schlenk Engineering College</div>
        <div class="edu-sub">Bachelor of Technology — Information Technology</div>
      </div>
      <div class="edu-meta">2023 – 2027<span class="cgpa">CGPA: 7.44 / 10</span></div>
    </div>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">03</span><h2>Experience</h2><div class="rule"></div></div>
    <div class="card">
      <div class="card-head">
        <span class="card-title">Infosys — Virtual Internship</span>
        <span class="card-date">Feb 2026</span>
      </div>
      <ul>
        <li>Developed a Smart Procurement &amp; Vendor Management System using Java and Spring Boot.</li>
        <li>Implemented vendor onboarding and centralized profile management modules.</li>
        <li>Automated procurement workflows with multi-level approval processes to improve efficiency.</li>
        <li>Built a real-time Purchase Order (PO) lifecycle tracking system for better monitoring and transparency.</li>
        <li>Integrated MySQL for optimized data storage, retrieval, and transaction management.</li>
      </ul>
    </div>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">04</span><h2>Projects</h2><div class="rule"></div></div>

    <div class="card">
      <div class="card-head">
        <span class="card-title">Technology Convergence Using BERT Topic Modeling &amp; Association Rule Mining</span>
        <span class="card-date">Nov 2025</span>
      </div>
      <ul>
        <li>Applied BERT for topic modelling on large text datasets.</li>
        <li>Used association rule mining to extract meaningful relationships and insights.</li>
      </ul>
    </div>

    <div class="card">
      <div class="card-head">
        <span class="card-title">Steel Furniture Manufacturing System</span>
        <span class="card-date">May 2025</span>
      </div>
      <ul>
        <li>Built a management system to handle orders, inventory, and production workflow.</li>
        <li>Improved operational efficiency and data record management.</li>
      </ul>
    </div>

    <div class="card">
      <div class="card-head">
        <span class="card-title">Route Optimization System</span>
        <span class="card-date">Mar 2026</span>
      </div>
      <ul>
        <li>Finds the most efficient path to travel between multiple locations, saving time, cost, and fuel.</li>
      </ul>
    </div>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">05</span><h2>Technical Skills</h2><div class="rule"></div></div>
    <div class="skill-grid">
      <div class="skill-cat">Languages</div>
      <div class="tag-row">
        <span class="tag">C</span><span class="tag">C++</span><span class="tag">Java</span><span class="tag">Python</span>
      </div>
      <div class="skill-cat">Web</div>
      <div class="tag-row">
        <span class="tag">HTML</span><span class="tag">CSS</span><span class="tag">JavaScript</span><span class="tag">React</span><span class="tag">Node.js</span>
      </div>
      <div class="skill-cat">Database</div>
      <div class="tag-row">
        <span class="tag">MySQL</span><span class="tag">MongoDB</span>
      </div>
      <div class="skill-cat">Concepts</div>
      <div class="tag-row">
        <span class="tag">OOP</span><span class="tag">DSA</span><span class="tag">DBMS</span>
      </div>
    </div>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">06</span><h2>Certifications</h2><div class="rule"></div></div>
    <ul class="plain-list">
      <li><span>NPTEL — Introduction to Internet of Things</span><span class="when">Nov 2024</span></li>
      <li><span>Infosys Springboard — Machine Learning Using Python</span><span class="when">May 2024</span></li>
      <li><span>Infosys Springboard — Java Foundation Certification</span><span class="when">Dec 2025</span></li>
    </ul>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">07</span><h2>Achievements</h2><div class="rule"></div></div>
    <ul class="plain-list">
      <li><span>Secured 3rd Prize — Yuvaa AI Stack Challenge 2026, for an AI-powered application.</span><span class="when">2026</span></li>
    </ul>
  </section>

  <section>
    <div class="sec-head"><span class="sec-tag">08</span><h2>Soft Skills</h2><div class="rule"></div></div>
    <div class="soft-row">
      <span class="soft">Problem Solving</span>
      <span class="soft">Teamwork</span>
      <span class="soft">Communication</span>
      <span class="soft">Time Management</span>
    </div>
  </section>

  <footer>// last updated · July 2026</footer>
</div>
</body>
</html>
