<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Yuvaraaj R K — Software Developer</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,600;9..144,700&family=Inter:wght@400;500;600;700&display=swap');

  :root{
    --navy:#1c2a44;
    --navy-deep:#101828;
    --gold:#a9812f;
    --paper:#faf8f4;
    --panel:#ffffff;
    --line:#e6e1d6;
    --muted:#6b7280;
    --text:#26303f;
  }

  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--paper);
    color:var(--text);
    font-family:'Inter',sans-serif;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
  }

  a{color:var(--navy);text-decoration:none;border-bottom:1px solid var(--line);}
  a:hover{border-bottom-color:var(--gold);color:var(--gold);}

  .wrap{
    max-width:860px;
    margin:0 auto;
    padding:56px 44px 70px;
  }

  /* ---------- HEADER ---------- */
  .header{
    display:flex;
    align-items:center;
    gap:26px;
    padding-bottom:32px;
    border-bottom:2px solid var(--navy);
    margin-bottom:36px;
  }
  .monogram{
    flex:0 0 auto;
    width:76px;height:76px;
    border-radius:50%;
    background:var(--navy);
    color:var(--paper);
    display:flex;align-items:center;justify-content:center;
    font-family:'Fraunces',serif;
    font-size:26px;
    font-weight:600;
    letter-spacing:0.02em;
    box-shadow:0 0 0 4px var(--paper), 0 0 0 5px var(--line);
  }
  .head-text h1{
    font-family:'Fraunces',serif;
    font-size:40px;
    font-weight:600;
    color:var(--navy-deep);
    margin:0 0 4px;
    letter-spacing:-0.01em;
  }
  .role{
    font-size:15px;
    font-weight:500;
    color:var(--gold);
    text-transform:uppercase;
    letter-spacing:0.08em;
    margin:0 0 12px;
  }
  .contact-row{
    display:flex;
    flex-wrap:wrap;
    gap:4px 20px;
    font-size:13px;
    color:var(--muted);
  }
  .contact-row a{color:var(--muted);border-bottom:none;}
  .contact-row a:hover{color:var(--gold);}
  .contact-row span::before{content:"•";color:var(--gold);margin-right:8px;font-size:11px;}
  .contact-row span:first-child::before{content:"";margin-right:0;}

  /* ---------- SECTIONS ---------- */
  section{margin-bottom:34px;}
  .sec-head{
    display:flex;
    align-items:center;
    gap:14px;
    margin-bottom:16px;
  }
  .sec-head h2{
    font-family:'Fraunces',serif;
    font-size:18px;
    font-weight:600;
    color:var(--navy-deep);
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
    color:#3d4757;
    max-width:70ch;
    font-style:italic;
    font-family:'Fraunces',serif;
    font-weight:500;
    line-height:1.65;
  }

  /* Education */
  .edu-row{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;
    gap:16px;
    flex-wrap:wrap;
    background:var(--panel);
    border:1px solid var(--line);
    border-left:3px solid var(--navy);
    border-radius:6px;
    padding:16px 20px;
  }
  .edu-name{
    font-family:'Fraunces',serif;
    font-weight:600;
    font-size:16.5px;
    color:var(--navy-deep);
  }
  .edu-sub{font-size:13.5px;color:var(--muted);margin-top:3px;}
  .edu-meta{
    text-align:right;
    font-size:13px;
    color:var(--navy);
    font-weight:600;
    white-space:nowrap;
  }
  .edu-meta .cgpa{display:block;color:var(--muted);font-weight:400;margin-top:3px;}

  /* Cards */
  .card{
    padding:18px 20px;
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:6px;
    margin-bottom:12px;
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
    font-family:'Fraunces',serif;
    font-weight:600;
    font-size:16px;
    color:var(--navy-deep);
  }
  .card-date{
    font-size:12px;
    font-weight:600;
    color:var(--gold);
    text-transform:uppercase;
    letter-spacing:0.05em;
    white-space:nowrap;
  }
  .card ul{
    margin:0;
    padding-left:18px;
    font-size:14px;
    color:#454f5f;
  }
  .card ul li{margin-bottom:5px;}
  .card ul li::marker{color:var(--gold);}

  /* Skills — image based */
  .skills-block{
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:6px;
    padding:22px 24px;
  }
  .skill-group{margin-bottom:18px;}
  .skill-group:last-child{margin-bottom:0;}
  .skill-label{
    font-size:12px;
    font-weight:600;
    text-transform:uppercase;
    letter-spacing:0.07em;
    color:var(--muted);
    margin-bottom:10px;
  }
  .skill-icons img{
    display:block;
    max-width:100%;
    height:auto;
  }

  /* Certifications / Achievements */
  .plain-list{list-style:none;margin:0;padding:0;background:var(--panel);border:1px solid var(--line);border-radius:6px;overflow:hidden;}
  .plain-list li{
    display:flex;
    justify-content:space-between;
    gap:12px;
    padding:13px 20px;
    border-bottom:1px solid var(--line);
    font-size:14px;
    color:#3d4757;
  }
  .plain-list li:last-child{border-bottom:none;}
  .plain-list .when{
    font-size:12px;
    font-weight:600;
    color:var(--gold);
    white-space:nowrap;
  }

  /* Soft skills */
  .soft-row{display:flex;flex-wrap:wrap;gap:10px;}
  .soft{
    font-size:13px;
    font-weight:500;
    padding:7px 16px;
    border-radius:20px;
    background:var(--navy);
    color:var(--paper);
  }

  footer{
    margin-top:44px;
    text-align:center;
    font-size:11px;
    color:var(--muted);
    letter-spacing:0.05em;
  }

  @media (max-width:600px){
    .wrap{padding:32px 20px 50px;}
    h1{font-size:30px;}
    .header{flex-direction:column;align-items:flex-start;gap:16px;}
    .edu-meta{text-align:left;}
  }

  @media print{
    body{background:#fff;}
    .wrap{max-width:100%;padding:18px 26px;}
    .card, .plain-list, .skills-block, .edu-row{border-color:#ddd;}
  }
</style>
</head>
<body>
<div class="wrap">

  <div class="header">
    <div class="monogram">YR</div>
    <div class="head-text">
      <h1>Yuvaraaj R K</h1>
      <p class="role">Software Developer · Full-Stack &amp; AI-Integrated Systems</p>
      <div class="contact-row">
        <span>Salem, Tamil Nadu</span>
        <span>+91 9994883043</span>
        <span><a href="mailto:yuvarajamanikkam@gmail.com">yuvarajamanikkam@gmail.com</a></span>
        <span><a href="https://github.com/yuvaraaj-29" target="_blank">GitHub</a></span>
        <span><a href="https://linkedin.com/in/yuvaraaj-r-k-556599357" target="_blank">LinkedIn</a></span>
      </div>
    </div>
  </div>

  <section>
    <div class="sec-head"><h2>Objective</h2><div class="rule"></div></div>
    <p class="objective">"Aspiring Software Developer with strong knowledge in Java, Python, and full-stack development — passionate about building scalable applications, automation systems, and AI-powered software solutions."</p>
  </section>

  <section>
    <div class="sec-head"><h2>Education</h2><div class="rule"></div></div>
    <div class="edu-row">
      <div>
        <div class="edu-name">Mepco Schlenk Engineering College</div>
        <div class="edu-sub">Bachelor of Technology — Information Technology</div>
      </div>
      <div class="edu-meta">2023 – 2027<span class="cgpa">CGPA: 7.44 / 10</span></div>
    </div>
  </section>

  <section>
    <div class="sec-head"><h2>Experience</h2><div class="rule"></div></div>
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
    <div class="sec-head"><h2>Projects</h2><div class="rule"></div></div>

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
    <div class="sec-head"><h2>Technical Skills</h2><div class="rule"></div></div>
    <div class="skills-block">
      <div class="skill-group">
        <div class="skill-label">Languages</div>
        <div class="skill-icons">
          <img src="https://skillicons.dev/icons?i=c,cpp,java,py" alt="C, C++, Java, Python" loading="lazy">
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-label">Web Technologies</div>
        <div class="skill-icons">
          <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs" alt="HTML, CSS, JavaScript, React, Node.js" loading="lazy">
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-label">Databases</div>
        <div class="skill-icons">
          <img src="https://skillicons.dev/icons?i=mysql,mongodb" alt="MySQL, MongoDB" loading="lazy">
        </div>
      </div>
      <div class="skill-group" style="margin-bottom:0;">
        <div class="skill-label">Core Concepts</div>
        <div class="soft-row">
          <span class="soft">OOP</span>
          <span class="soft">Data Structures &amp; Algorithms</span>
          <span class="soft">DBMS</span>
        </div>
      </div>
    </div>
  </section>

  <section>
    <div class="sec-head"><h2>Certifications</h2><div class="rule"></div></div>
    <ul class="plain-list">
      <li><span>NPTEL — Introduction to Internet of Things</span><span class="when">Nov 2024</span></li>
      <li><span>Infosys Springboard — Machine Learning Using Python</span><span class="when">May 2024</span></li>
      <li><span>Infosys Springboard — Java Foundation Certification</span><span class="when">Dec 2025</span></li>
    </ul>
  </section>

  <section>
    <div class="sec-head"><h2>Achievements</h2><div class="rule"></div></div>
    <ul class="plain-list">
      <li><span>Secured 3rd Prize — Yuvaa AI Stack Challenge 2026, for an AI-powered application.</span><span class="when">2026</span></li>
    </ul>
  </section>

  <section>
    <div class="sec-head"><h2>Soft Skills</h2><div class="rule"></div></div>
    <div class="soft-row">
      <span class="soft">Problem Solving</span>
      <span class="soft">Teamwork</span>
      <span class="soft">Communication</span>
      <span class="soft">Time Management</span>
    </div>
  </section>

  <footer>LAST UPDATED · JULY 2026</footer>
</div>
</body>
</html>
