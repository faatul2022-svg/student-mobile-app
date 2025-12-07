<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>My Mobile App — Project Website + 5-minute Presentation</title>
  <style>
    :root{--accent:#2b6cb0;--bg:#f7fafc;--card:#fff;--muted:#6b7280}
    body{font-family:Inter,system-ui,Segoe UI,Arial;background:var(--bg);color:#111;margin:0}
    .wrap{max-width:980px;margin:28px auto;padding:20px}
    header{display:flex;align-items:center;gap:16px}
    .logo{width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#805ad5);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700}
    h1{margin:0;font-size:20px}
    p.lead{color:var(--muted);margin:6px 0 18px}
    .grid{display:grid;grid-template-columns:1fr 340px;gap:18px}
    .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(15,23,42,0.06)}
    .screenshot{width:100%;height:220px;border-radius:10px;background:repeating-linear-gradient(45deg,#eef2ff 0 10px, #fff 10px 20px);display:flex;align-items:center;justify-content:center;color:var(--muted)}
    .features ul{padding-left:18px;margin:8px 0}
    .cta{display:flex;gap:8px;margin-top:12px}
    .btn{padding:10px 12px;border-radius:10px;border:0;background:var(--accent);color:#fff;cursor:pointer}
    .btn.secondary{background:#edf2ff;color:var(--accent);border:1px solid rgba(43,108,176,0.12)}
    .meta{font-size:13px;color:var(--muted)}
    /* Presentation area */
    .presentation{display:flex;flex-direction:column;gap:12px}
    .slides{background:#0f172a;color:#fff;border-radius:10px;padding:18px;height:300px;display:flex;flex-direction:column;justify-content:center;align-items:center}
    .slide-title{font-size:22px;margin:0}
    .slide-body{margin-top:8px;color:#d1d5db}
    .controls{display:flex;gap:8px;justify-content:center;margin-top:8px}
    .note{background:#fff;padding:12px;border-radius:8px;color:#111;max-height:150px;overflow:auto}
    .qa{display:flex;flex-direction:column;gap:8px}
    .qa .q{font-weight:600}
    footer{margin-top:20px;text-align:center;color:var(--muted);font-size:13px}
    @media (max-width:900px){.grid{grid-template-columns:1fr;}.slides{height:260px}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">AP</div>
      <div>
        <h1>Mobile App Project — Website + 5‑Minute Q&A Presentation</h1>
        <p class="lead">One-page website to show your project; interactive built-in slides and speaker notes for a 5‑minute classroom presentation with practice Q&A.</p>
      </div>
    </header>

    <div class="grid">
      <main>
        <section class="card">
          <h2>Project at a glance</h2>
          <div class="screenshot">Add your app screenshot(s) here</div>
          <p class="meta">Short description: A one-sentence summary (e.g. "Taskly — a simple task manager for students to plan and share study tasks").</p>

          <div style="margin-top:12px" class="features">
            <h3>Key features</h3>
            <ul>
              <li>Fast onboarding and clean UI</li>
              <li>Offline sync + push notifications</li>
              <li>Shareable study lists and quick collaboration</li>
            </ul>
          </div>

          <div style="margin-top:10px" class="cta">
            <button class="btn" onclick="alert('Replace with your demo link or APK/App Store link')">Open demo</button>
            <button class="btn secondary" onclick="alert('Replace with GitHub repo link')">View code</button>
          </div>
        </section>

        <section class="card" style="margin-top:14px">
          <h3>How to use this page</h3>
          <ol>
            <li>Add your screenshots and update the short description.</li>
            <li>Set the demo / repo links on the buttons.</li>
            <li>Use the <strong>Presentation</strong> area to rehearse — speaker notes and practice Q&amp;A included.</li>
          </ol>
        </section>

        <section class="card" style="margin-top:14px">
          <h3>Hosting suggestions</h3>
          <p class="meta">Quick hosts: GitHub Pages, Netlify, or Vercel. Just push this file as <code>index.html</code> and point the site.</p>
        </section>

      </main>

      <aside>
        <div class="card presentation">
          <h3>Presentation (5 minutes)</h3>
          <div id="slides" class="slides">
            <div id="slide-title" class="slide-title">Slide 1 — Title & Team</div>
            <div id="slide-body" class="slide-body">Project name • Your name • 30s: quick hook — why this matters</div>
          </div>

          <div class="controls">
            <button class="btn secondary" onclick="prevSlide()">◀ Prev</button>
            <button class="btn" onclick="nextSlide()">Next ▶</button>
            <button class="btn secondary" onclick="toggleNotes()">Toggle notes</button>
          </div>

          <div id="notes" class="note" style="display:none">Speaker notes show here.</div>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>Practice Q&amp;A</h3>
          <div class="qa">
            <div>
              <div class="q">Q1: What problem does the app solve?</div>
              <div class="a">A1: Brief answer (15s): the app helps [target users] to solve [problem] by [main idea].</div>
            </div>

            <div>
              <div class="q">Q2: What are the main features?</div>
              <div class="a">A2: Feature list: 1) X, 2) Y, 3) Z — mention one technical highlight (e.g., offline sync).</div>
            </div>

            <div>
              <div class="q">Q3: Which technologies did you use?</div>
              <div class="a">A3: E.g. React Native / Flutter, Firebase / REST API, SQLite. One sentence per tech.</div>
            </div>

            <div>
              <div class="q">Q4: How did you test or validate it?</div>
              <div class="a">A4: Short: conducted N user tests, measured X metric, fixed Y bugs.</div>
            </div>

            <div>
              <div class="q">Q5: What are next steps?</div>
              <div class="a">A5: Short roadmap: polish UI, add auth, release beta, gather feedback.</div>
            </div>

            <div>
              <div class="q">Practice tip</div>
              <div class="a">Keep answers to ~20–30 seconds during class Q&amp;A. If you don't know, offer to follow up via email.</div>
            </div>

          </div>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>Presenter checklist</h3>
          <ul>
            <li>Practice 2× full runs — time each run to 5 minutes</li>
            <li>Prepare 1-minute demo (if allowed) or recorded screen</li>
            <li>Have backup PDF of slides (in case of browser issues)</li>
          </ul>
        </div>

      </aside>
    </div>

    <footer>
      <small>Generated template • Edit texts and links to match your project. Need customization? Reply and I'll edit the page or create a PPTX for you.</small>
    </footer>
  </div>

  <script>
    const slides = [
      {
        title: 'Slide 1 — Title & Hook (30s)',
        body: 'Project name • Your name • Hook: one sentence why this matters',
        notes: 'Say: Hello, I am NAME. Our app solves XYZ. Hook: a short surprising fact or pain point.'
      },
      {
        title: 'Slide 2 — Problem & Target (60s)',
        body: 'Explain the problem and who suffers from it. One brief example or story.',
        notes: 'Be concise. Use a concrete user story ("A student who..."), keep to 45–60s.'
      },
      {
        title: 'Slide 3 — Solution & Key features (60s)',
        body: 'Show the app and 3 main features. Mention one technical highlight.',
        notes: 'Quick demo lines: open app, show feature X, mention offline sync or fast search.'
      },
      {
        title: 'Slide 4 — Tech & Validation (60s)',
        body: 'Which tech you used + how you tested it (users / metrics).',
        notes: 'Mention frameworks, backend, database, tests, and what you learned.'
      },
      {
        title: 'Slide 5 — Demo / Next steps / CTA (60s)',
        body: 'Short demo or screenshots. Next steps and how instructor/class can help.',
        notes: 'End with a clear ask: feedback, permission to test with classmates, or GitHub link.'
      },
      {
        title: 'Q&A — Be ready (remaining time)',
        body: 'Open for questions. Use the practice Q&A on the right.',
        notes: 'Repeat question briefly, answer concisely, offer to follow up if detailed.'
      }
    ];

    let idx = 0;
    const titleEl = document.getElementById('slide-title');
    const bodyEl = document.getElementById('slide-body');
    const notesEl = document.getElementById('notes');

    function render() {
      const s = slides[idx];
      titleEl.textContent = s.title;
      bodyEl.textContent = s.body;
      notesEl.textContent = s.notes;
    }
    function nextSlide(){ idx = Math.min(idx+1, slides.length-1); render(); }
    function prevSlide(){ idx = Math.max(idx-1, 0); render(); }
    function toggleNotes(){ notesEl.style.display = notesEl.style.display === 'none' ? 'block' : 'none'; }
    render();
  </script>
</body>
</html>
