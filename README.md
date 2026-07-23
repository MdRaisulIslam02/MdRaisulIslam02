
<style>
  @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&family=Inter:wght@400;500;600&display=swap');
  *{box-sizing:border-box;margin:0;padding:0}
  .wrap{font-family:'Inter',sans-serif;background:#0d1117;color:#e6edf3;min-height:600px;padding:2rem 1.5rem;max-width:860px;margin:0 auto}
  .badge-row{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:1.5rem;justify-content:center}
  .badge{background:#1f6feb;color:#fff;font-size:11px;font-weight:600;padding:4px 12px;border-radius:6px;letter-spacing:.5px;text-transform:uppercase}
  .badge.green{background:#238636}
  .badge.gray{background:#30363d;color:#8b949e}
  .typing-line{font-family:'Fira Code',monospace;font-size:22px;font-weight:600;color:#58a6ff;text-align:center;margin-bottom:.3rem;letter-spacing:-0.5px}
  .sub-line{text-align:center;color:#8b949e;font-size:13px;margin-bottom:2rem;font-family:'Fira Code',monospace}
  .grid2{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1.5rem}
  .card{background:#161b22;border:1px solid #30363d;border-radius:12px;padding:1.25rem}
  .card h3{font-size:13px;color:#8b949e;text-transform:uppercase;letter-spacing:1px;margin-bottom:.8rem;font-weight:500}
  .code-block{background:#0d1117;border:1px solid #30363d;border-radius:8px;padding:1rem;font-family:'Fira Code',monospace;font-size:11.5px;line-height:1.8;color:#e6edf3}
  .kw{color:#ff7b72}.str{color:#a5d6ff}.prop{color:#79c0ff}.val{color:#ffa657}
  .bullet-list{list-style:none;display:flex;flex-direction:column;gap:.6rem}
  .bullet-list li{display:flex;align-items:flex-start;gap:.5rem;font-size:13px;color:#c9d1d9;line-height:1.5}
  .dot{width:6px;height:6px;border-radius:50%;background:#58a6ff;flex-shrink:0;margin-top:5px}
  .dot.green{background:#3fb950}
  .dot.purple{background:#a371f7}
  .dot.orange{background:#ffa657}
  .section-title{font-size:13px;color:#8b949e;text-transform:uppercase;letter-spacing:1px;margin:1.5rem 0 .8rem;font-weight:500;display:flex;align-items:center;gap:.5rem}
  .section-title::after{content:'';flex:1;height:1px;background:#30363d}
  .tech-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(100px,1fr));gap:8px;margin-bottom:1.5rem}
  .tech-chip{background:#161b22;border:1px solid #30363d;border-radius:8px;padding:8px 10px;display:flex;align-items:center;gap:8px;font-size:12px;color:#c9d1d9;font-weight:500}
  .tech-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0}
  .projects-table{width:100%;border-collapse:collapse;font-size:12.5px}
  .projects-table th{text-align:left;color:#8b949e;font-weight:500;padding:6px 10px;border-bottom:1px solid #30363d;font-size:11px;text-transform:uppercase;letter-spacing:.5px}
  .projects-table td{padding:8px 10px;border-bottom:1px solid #21262d;color:#c9d1d9;vertical-align:middle}
  .projects-table tr:last-child td{border-bottom:none}
  .impact-badge{background:#1a2e1a;color:#3fb950;font-size:11px;padding:2px 8px;border-radius:6px;font-weight:500;border:1px solid #238636;white-space:nowrap}
  .stat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:1.5rem}
  .stat-card{background:#161b22;border:1px solid #30363d;border-radius:10px;padding:1rem;text-align:center}
  .stat-num{font-size:22px;font-weight:600;color:#58a6ff;font-family:'Fira Code',monospace}
  .stat-label{font-size:11px;color:#8b949e;margin-top:4px;text-transform:uppercase;letter-spacing:.5px}
  .social-row{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-bottom:1.5rem}
  .social-chip{background:#161b22;border:1px solid #30363d;border-radius:8px;padding:6px 14px;font-size:12px;color:#c9d1d9;font-weight:500;display:flex;align-items:center;gap:6px;cursor:pointer;transition:border-color .15s,color .15s}
  .social-chip:hover{border-color:#58a6ff;color:#58a6ff}
  .lang-bar-wrap{margin-bottom:1.5rem}
  .lang-row{display:flex;align-items:center;gap:10px;margin-bottom:8px}
  .lang-name{font-size:12px;color:#c9d1d9;width:110px;flex-shrink:0}
  .lang-bar-bg{flex:1;height:6px;background:#21262d;border-radius:4px;overflow:hidden}
  .lang-bar{height:100%;border-radius:4px}
  .lang-pct{font-size:11px;color:#8b949e;width:36px;text-align:right;flex-shrink:0;font-family:'Fira Code',monospace}
  .footer{text-align:center;color:#484f58;font-size:11px;font-family:'Fira Code',monospace;padding-top:1rem;border-top:1px solid #21262d;margin-top:.5rem}
  .streak-row{display:flex;gap:8px;margin-bottom:1.5rem;justify-content:space-between}
  .streak-box{background:#161b22;border:1px solid #30363d;border-radius:10px;padding:.9rem 1rem;flex:1;text-align:center}
  .streak-val{font-size:18px;font-weight:600;color:#ffa657;font-family:'Fira Code',monospace}
  .streak-lbl{font-size:10px;color:#8b949e;margin-top:3px;text-transform:uppercase;letter-spacing:.5px}
  .avatar{width:44px;height:44px;border-radius:50%;background:linear-gradient(135deg,#1f6feb,#a371f7);display:flex;align-items:center;justify-content:center;font-size:16px;font-weight:700;color:#fff;flex-shrink:0}
  .header-top{display:flex;align-items:center;gap:12px;justify-content:center;margin-bottom:.5rem}
</style>

<div class="wrap">
  <div class="header-top">
    <div class="avatar">R</div>
    <div>
      <div class="typing-line">Raisul Islam</div>
      <div class="sub-line">MERN Stack Developer · Bangladesh 🇧🇩</div>
    </div>
  </div>

  <div class="badge-row">
    <span class="badge">MERN Stack</span>
    <span class="badge green">Open to Work</span>
    <span class="badge gray">📍 Bangladesh</span>
    <span class="badge gray">📧 coder.raisul@gmail.com</span>
  </div>

  <div class="grid2">
    <div class="card">
      <h3>About</h3>
      <div class="code-block">
<span class="kw">const</span> <span class="prop">raisul</span> = {<br>
&nbsp;&nbsp;<span class="prop">role</span>: <span class="str">"MERN Developer"</span>,<br>
&nbsp;&nbsp;<span class="prop">location</span>: <span class="str">"Bangladesh 🇧🇩"</span>,<br>
&nbsp;&nbsp;<span class="prop">focus</span>: <span class="str">"Scalable Web Apps"</span>,<br>
&nbsp;&nbsp;<span class="prop">funFact</span>: <span class="str">"console.log is<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;comfort food"</span><br>
}
      </div>
    </div>
    <div class="card">
      <h3>What I do</h3>
      <ul class="bullet-list">
        <li><span class="dot"></span>Build full-stack apps end-to-end with <strong style="color:#58a6ff">MERN</strong></li>
        <li><span class="dot green"></span>Co-founder of <strong style="color:#3fb950">Analyzen</strong> — BD's largest IT agency</li>
        <li><span class="dot purple"></span>Creator of <strong style="color:#a371f7">Listenyzen</strong> AI SaaS platform</li>
        <li><span class="dot orange"></span>Programming tutor — <strong style="color:#ffa657">1K+ active learners</strong></li>
      </ul>
    </div>
  </div>

  <div class="section-title">Tech Stack</div>
  <div class="tech-grid">
    <div class="tech-chip"><span class="tech-dot" style="background:#4CAF50"></span>MongoDB</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#8BC34A"></span>Express.js</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#61DAFB"></span>React</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#43A047"></span>Node.js</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#fff"></span>Next.js</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#3178C6"></span>TypeScript</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#38BDF8"></span>Tailwind</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#F7DF1E"></span>JavaScript</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#00758F"></span>MySQL</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#8892BE"></span>PHP</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#F05032"></span>Git</div>
    <div class="tech-chip"><span class="tech-dot" style="background:#F24E1E"></span>Figma</div>
  </div>

  <div class="section-title">Impact Numbers</div>
  <div class="stat-grid">
    <div class="stat-card"><div class="stat-num">120+</div><div class="stat-label">Agency Clients</div></div>
    <div class="stat-card"><div class="stat-num">2.5K+</div><div class="stat-label">BATB Distributors</div></div>
    <div class="stat-card"><div class="stat-num">1K+</div><div class="stat-label">Active Learners</div></div>
  </div>

  <div class="section-title">Projects & Ventures</div>
  <div class="card" style="margin-bottom:1.5rem">
    <table class="projects-table">
      <thead>
        <tr><th>Project</th><th>Description</th><th>Impact</th></tr>
      </thead>
      <tbody>
        <tr>
          <td><span style="color:#58a6ff;font-weight:500">Analyzen</span></td>
          <td>BD's first & largest IT agency</td>
          <td><span class="impact-badge">120+ clients</span></td>
        </tr>
        <tr>
          <td><span style="color:#a371f7;font-weight:500">Listenyzen</span></td>
          <td>AI-powered social media analytics SaaS</td>
          <td><span class="impact-badge">16+ clients</span></td>
        </tr>
        <tr>
          <td><span style="color:#ffa657;font-weight:500">Prism ERP</span></td>
          <td>Sales automation for British American Tobacco BD</td>
          <td><span class="impact-badge">2.5K+ distributors</span></td>
        </tr>
        <tr>
          <td><span style="color:#3fb950;font-weight:500">Raisul Islam</span></td>
          <td>Programming learning platform for Bangladesh</td>
          <td><span class="impact-badge">1K+ learners</span></td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="section-title">Top Languages</div>
  <div class="lang-bar-wrap">
    <div class="lang-row"><span class="lang-name">JavaScript</span><div class="lang-bar-bg"><div class="lang-bar" style="width:72%;background:#F7DF1E"></div></div><span class="lang-pct">72%</span></div>
    <div class="lang-row"><span class="lang-name">TypeScript</span><div class="lang-bar-bg"><div class="lang-bar" style="width:55%;background:#3178C6"></div></div><span class="lang-pct">55%</span></div>
    <div class="lang-row"><span class="lang-name">CSS</span><div class="lang-bar-bg"><div class="lang-bar" style="width:40%;background:#264de4"></div></div><span class="lang-pct">40%</span></div>
    <div class="lang-row"><span class="lang-name">PHP</span><div class="lang-bar-bg"><div class="lang-bar" style="width:25%;background:#8892BE"></div></div><span class="lang-pct">25%</span></div>
    <div class="lang-row"><span class="lang-name">HTML</span><div class="lang-bar-bg"><div class="lang-bar" style="width:18%;background:#E34C26"></div></div><span class="lang-pct">18%</span></div>
  </div>

  <div class="section-title">Connect</div>
  <div class="social-row">
    <div class="social-chip">🔗 LinkedIn</div>
    <div class="social-chip">📘 Facebook</div>
    <div class="social-chip">🎥 YouTube</div>
    <div class="social-chip">📸 Instagram</div>
    <div class="social-chip">🐦 Twitter</div>
    <div class="social-chip">📧 Gmail</div>
  </div>

  <div class="footer">
    💻 MERN Stack Developer &nbsp;|&nbsp; 📺 Content Creator &nbsp;|&nbsp; 🇧🇩 Bangladesh<br/>
    Thanks for stopping by — check out my pinned repos below ⭐
  </div>
</div>
