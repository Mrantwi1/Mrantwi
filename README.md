<!--
GitHub Profile Revamp — HTML Template
Usage:
 - This file is a standalone HTML template to preview a professional GitHub profile page (or use as content for a GitHub Pages site).
 - Replace all {{PLACEHOLDERS}} with your own info (name, bio, links, projects, images).
 - If you want to use this as a README.md on GitHub, convert sections to Markdown and preserve the text content. GitHub README supports some HTML but Markdown is often easier.

Sections included:
 - Header with name, title, and social links
 - About / Story
 - Key Metrics / Quick Stats
 - Skills (languages, frameworks, tools)
 - Featured Projects (card layout)
 - Experience / Education (timeline)
 - Contributions & Open Source (how to contribute)
 - Contact & Call to Action
 - Footer with badges and optional extra links
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>{Kwame Antwi Boasiako} — Back-end Developer | GitHub Profile</title>
  <style>
    :root{--bg:#0f1720;--card:#0b1220;--muted:#94a3b8;--accent:#06b6d4;--glass:rgba(255,255,255,0.04)}
    *{box-sizing:border-box;font-family:Inter,-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,'Helvetica Neue',Arial}
    body{margin:0;background:linear-gradient(180deg,#071226 0%, #041025 100%);color:#e6eef8;line-height:1.5}
    .container{max-width:980px;margin:40px auto;padding:28px}
    header{display:flex;gap:20px;align-items:center}
    .avatar{width:110px;height:110px;border-radius:18px;overflow:hidden;border:2px solid rgba(255,255,255,0.06);flex:0 0 110px}
    .avatar img{width:100%;height:100%;object-fit:cover}
    .title{flex:1}
    h1{margin:0;font-size:26px}
    .subtitle{color:var(--muted);margin-top:6px}
    .social{margin-top:12px;display:flex;gap:10px}
    .pill{background:var(--glass);padding:6px 10px;border-radius:999px;font-size:13px;color:var(--muted);display:inline-flex;align-items:center;gap:8px}

    .grid{display:grid;grid-template-columns:1fr 320px;gap:20px;margin-top:28px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:14px;border:1px solid rgba(255,255,255,0.03)}
    .skills{display:flex;flex-wrap:wrap;gap:10px}
    .skill{background:rgba(255,255,255,0.03);padding:8px 10px;border-radius:8px;font-size:13px;color:var(--muted)}

    .projects{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
    .proj{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02));padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);display:flex;flex-direction:column}
    .proj h3{margin:0 0 8px 0;font-size:15px}
    .proj p{margin:0;color:var(--muted);font-size:13px}
    .tags{margin-top:10px;display:flex;gap:8px;flex-wrap:wrap}
    .tag{background:rgba(255,255,255,0.03);padding:6px 8px;border-radius:8px;font-size:12px;color:var(--muted)}

    aside .card + .card{margin-top:14px}
    .metrics{display:flex;gap:12px;flex-wrap:wrap}
    .metric{background:rgba(255,255,255,0.02);padding:12px;border-radius:10px;min-width:120px;text-align:center}
    .metric strong{display:block;font-size:18px}

    .timeline{display:flex;flex-direction:column;gap:12px}
    .time-item{padding:10px;border-radius:10px;background:rgba(255,255,255,0.01);border-left:3px solid rgba(255,255,255,0.03)}
    .cta{display:flex;gap:10px;align-items:center;margin-top:12px}
    .btn{background:linear-gradient(90deg,var(--accent),#0ea5a1);color:#042027;padding:10px 14px;border-radius:10px;font-weight:600;text-decoration:none}
    .ghost{border:1px solid rgba(255,255,255,0.06);padding:10px 14px;border-radius:10px;color:var(--muted);text-decoration:none}

    footer{margin-top:28px;color:var(--muted);font-size:13px;text-align:center}

    /* responsive */
    @media (max-width:900px){.grid{grid-template-columns:1fr}.projects{grid-template-columns:1fr}.avatar{width:86px;height:86px}.container{padding:16px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="avatar">
        <!-- Replace src with your photo or GitHub avatar URL -->
        <img src="https://avatars.githubusercontent.com/{{GITHUB_USERNAME}}" alt="{{NAME}} avatar" />
      </div>
      <div class="title">
        <h1>{{Kwame Antwi Boasiako}} <span style="color:var(--accent);font-weight:600">| Back-end Developer</span></h1>
        <div class="subtitle">ALX Back-end learner • Building dependable, scalable server-side systems • Open-source contributor</div>
        <div class="social">
          <a class="pill" href="https://github.com/{{GITHUB_USERNAME}}">GitHub</a>
          <a class="pill" href="https://www.linkedin.com/in/{{LINKEDIN}}">LinkedIn</a>
          <a class="pill" href="mailto:{{EMAIL}}">Email</a>
        </div>
      </div>
    </header>

    <div class="grid">
      <main>
        <section class="card">
          <h2 style="margin-top:0">About me</h2>
          <p style="color:var(--muted);margin-top:10px">I started software engineering because <strong>{{WHY_SOFTWARE_ENGINEERING}}</strong>. I’m passionate about server-side systems, APIs, performance, and designing clear, testable code. My goal is to become a top back-end engineer by building real-world projects, contributing to open source, and learning system design.</p>

          <div style="margin-top:16px" class="metrics">
            <div class="metric"><strong>{{YEARS}}</strong><small>Years coding</small></div>
            <div class="metric"><strong>{{REPOS}}</strong><small>Public repos</small></div>
            <div class="metric"><strong>{{CONTRIBS}}</strong><small>Contributions this year</small></div>
          </div>
        </section>

        <section class="card" style="margin-top:16px">
          <h2>Featured Projects</h2>
          <p style="color:var(--muted);margin-top:6px">Shortlist of production-like projects that show problem-solving, architecture, testing and deployment.</p>

          <div class="projects" style="margin-top:12px">
            <!-- Project Card: duplicate & replace content -->
            <article class="proj">
              <h3><a href="https://github.com/{{GITHUB_USERNAME}}/{{PROJECT1_REPO}}" style="color:inherit;text-decoration:none">{{PROJECT1_NAME}}</a></h3>
              <p>{{PROJECT1_ONE_LINE}}</p>
              <div class="tags">
                <span class="tag">Node.js</span>
                <span class="tag">Postgres</span>
                <span class="tag">Docker</span>
              </div>
            </article>

            <article class="proj">
              <h3><a href="https://github.com/{{GITHUB_USERNAME}}/{{PROJECT2_REPO}}" style="color:inherit;text-decoration:none">{{PROJECT2_NAME}}</a></h3>
              <p>{{PROJECT2_ONE_LINE}}</p>
              <div class="tags">
                <span class="tag">Python</span>
                <span class="tag">FastAPI</span>
                <span class="tag">Redis</span>
              </div>
            </article>

            <!-- Add more project cards as needed -->
          </div>
        </section>

        <section class="card" style="margin-top:16px">
          <h2>Skills & Tools</h2>
          <div style="margin-top:10px" class="skills">
            <!-- Replace with your real skills -->
            <span class="skill">JavaScript (Node.js)</span>
            <span class="skill">Python</span>
            <span class="skill">SQL & Postgres</span>
            <span class="skill">REST & GraphQL</span>
            <span class="skill">Docker</span>
            <span class="skill">Kubernetes (basics)</span>
            <span class="skill">CI/CD (GitHub Actions)</span>
            <span class="skill">Testing (Jest / Pytest)</span>
          </div>
        </section>

        <section class="card" style="margin-top:16px">
          <h2>Experience & Education</h2>
          <div class="timeline" style="margin-top:10px">
            <div class="time-item">
              <strong>Back-end Intern / ALX Projects</strong>
              <div style="color:var(--muted);font-size:13px">{{DATE_RANGE}}</div>
              <div style="margin-top:6px;color:var(--muted);font-size:13px">Worked on building scalable APIs, deploying containers, and implementing unit & integration tests.</div>
            </div>

            <div class="time-item">
              <strong>{{UNIVERSITY_OR_BOOTCAMP}}</strong>
              <div style="color:var(--muted);font-size:13px">{{EDU_DATE}}</div>
              <div style="margin-top:6px;color:var(--muted);font-size:13px">Studied computer science fundamentals, data structures, and algorithms.</div>
            </div>
          </div>
        </section>

      </main>

      <aside>
        <div class="card">
          <h3>Quick links</h3>
          <ul style="padding-left:18px;color:var(--muted);margin-top:8px">
            <li><a href="https://github.com/{{GITHUB_USERNAME}}?tab=repositories" style="color:inherit">All repos</a></li>
            <li><a href="https://github.com/{{GITHUB_USERNAME}}?tab=followers" style="color:inherit">Followers</a></li>
            <li><a href="https://github.com/{{GITHUB_USERNAME}}/{{PROJECT1_REPO}}" style="color:inherit">Featured project 1</a></li>
          </ul>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>Open Source & Contributions</h3>
          <p style="color:var(--muted);font-size:13px">How to contribute: fork → branch → PR. Look for `good-first-issue` and `help wanted` labels. Include tests, and a clear PR description.</p>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>Reach out</h3>
          <p style="color:var(--muted);font-size:13px">Interested in collaborating or hiring? Let’s connect.</p>
          <div class="cta">
            <a class="btn" href="mailto:{{EMAIL}}">Email me</a>
            <a class="ghost" href="https://calendly.com/{{CALENDLY}}">Book time</a>
          </div>
        </div>

      </aside>
    </div>

    <footer>
      <div style="margin-bottom:8px">Pro tip: Keep your README/Pages up-to-date — add a short story for each featured project that explains the tradeoffs and your technical decisions.</div>
      <div style="font-size:12px;color:var(--muted)">Made with ❤️ • ALX learner • Last updated: {{LAST_UPDATED_DATE}}</div>
    </footer>
  </div>
</body>
</html>
