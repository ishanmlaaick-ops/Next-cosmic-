# Next-cosmic-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Cosmic Nexus — Engineered by Ishan</title>
  <meta name="description" content="Transform ideas into polished, ready-to-use creative outputs—prompts, scripts, thumbnails, SEO—with the precision and artistry of Ishan." />
  <meta name="theme-color" content="#0b0f1a" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://unpkg.com/balloon-css/balloon.min.css">
  <style>
    :root {
      --bg: #070a12;
      --bg-2: #0d1220;
      --text: #e7ecff;
      --muted: #a9b3d3;
      --accent: #7aa2ff;
      --accent-2: #9e7aff;
      --success: #4ade80;
      --warning: #f59e0b;
      --danger: #ef4444;
      --card: rgba(255,255,255,0.06);
      --glass: rgba(255,255,255,0.08);
      --border: rgba(255,255,255,0.12);
      --shadow: 0 10px 30px rgba(0,0,0,0.45), inset 0 0 0 1px var(--border);
    }
    [data-theme="light"] {
      --bg: #f8fafc;
      --bg-2: #eef2ff;
      --text: #0b1020;
      --muted: #3b445a;
      --accent: #3b82f6;
      --accent-2: #7c3aed;
      --card: rgba(0,0,0,0.04);
      --glass: rgba(255,255,255,0.6);
      --border: rgba(0,0,0,0.08);
      --shadow: 0 8px 24px rgba(0,0,0,0.08), inset 0 0 0 1px var(--border);
    }

    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0;
      background: radial-gradient(1200px 800px at 20% 10%, #0d1330 0%, var(--bg) 50%),
                  radial-gradient(900px 700px at 90% 20%, #181a3a 0%, transparent 60%),
                  radial-gradient(1400px 1000px at 50% 100%, #12162b 0%, transparent 60%);
      color: var(--text);
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      line-height: 1.6;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }

    /* Global layout */
    .container { width: 100%; max-width: 1200px; margin: 0 auto; padding: 0 24px; }
    section { padding: 96px 0; position: relative; }

    /* Header */
    header {
      position: sticky; top: 0; z-index: 50;
      backdrop-filter: saturate(160%) blur(8px);
      background: linear-gradient(to bottom, rgba(0,0,0,0.35), rgba(0,0,0,0.0));
      border-bottom: 1px solid var(--border);
    }
    .nav {
      display: flex; align-items: center; justify-content: space-between;
      padding: 16px 0;
    }
    .brand {
      display: flex; align-items: center; gap: 12px; font-weight: 700; letter-spacing: 0.4px;
    }
    .brand-logo {
      width: 36px; height: 36px; border-radius: 10px;
      background: conic-gradient(from 210deg, #9e7aff, #7aa2ff, #34d399, #f59e0b, #9e7aff);
      box-shadow: 0 0 18px rgba(122,162,255,0.6);
    }
    .nav-links {
      display: flex; gap: 16px; align-items: center;
    }
    .nav-links a {
      color: var(--muted); text-decoration: none; font-weight: 500; padding: 8px 12px; border-radius: 8px;
    }
    .nav-links a:hover { background: var(--card); color: var(--text); }
    .btn {
      padding: 10px 16px; border-radius: 10px; border: 1px solid var(--border);
      background: linear-gradient(180deg, var(--card), transparent);
      color: var(--text); cursor: pointer; font-weight: 600; letter-spacing: 0.2px;
      transition: transform .15s ease, box-shadow .15s ease, background .2s ease;
      box-shadow: var(--shadow);
    }
    .btn:hover { transform: translateY(-1px); }
    .btn.primary {
      background: linear-gradient(180deg, var(--accent), var(--accent-2));
      border: none; color: white; box-shadow: 0 12px 30px rgba(122,162,255,0.35);
    }
    .theme-toggle {
      display: inline-flex; align-items: center; gap: 8px; padding: 8px 12px; border-radius: 10px; cursor: pointer;
      border: 1px solid var(--border); background: var(--card);
    }

    /* Hero */
    .hero {
      padding: 120px 0 80px; overflow: hidden;
    }
    .galaxy {
      position: absolute; inset: 0; pointer-events: none; z-index: -1; opacity: 0.7;
      background:
        radial-gradient(800px 800px at 20% 30%, rgba(122,162,255,0.22), transparent 60%),
        radial-gradient(600px 600px at 80% 20%, rgba(158,122,255,0.18), transparent 65%),
        radial-gradient(900px 900px at 50% 80%, rgba(52,211,153,0.14), transparent 60%);
      animation: pulse 8s ease-in-out infinite;
    }
    @keyframes pulse { 0%,100% { filter: hue-rotate(0deg); } 50% { filter: hue-rotate(18deg); } }
    .hero-grid {
      display: grid; grid-template-columns: 1.2fr 1fr; gap: 40px; align-items: center;
    }
    .hero h1 {
      font-family: "Space Grotesk", Inter, sans-serif;
      font-size: clamp(34px, 5vw, 58px); line-height: 1.05; margin: 0 0 18px;
      letter-spacing: -0.5px;
    }
    .hero p { color: var(--muted); font-size: clamp(16px, 1.2vw, 18px); }
    .cta-row { display: flex; gap: 12px; margin-top: 24px; flex-wrap: wrap; }
    .orb {
      width: 420px; height: 420px; border-radius: 50%;
      background: radial-gradient(circle at 30% 30%, #9e7aff 0%, #7aa2ff 40%, #0ea5e9 60%, #111827 68%);
      filter: saturate(120%) contrast(110%);
      box-shadow: 0 25px 80px rgba(126, 153, 255, 0.35), inset 0 0 120px rgba(0,0,0,0.35);
      position: relative; transform: perspective(1200px) rotateX(14deg) rotateY(-10deg);
      animation: float 6s ease-in-out infinite;
    }
    @keyframes float { 0%,100% { transform: perspective(1200px) rotateX(14deg) rotateY(-10deg) translateY(0); } 50% { transform: perspective(1200px) rotateX(16deg) rotateY(-12deg) translateY(-12px); } }
    .orb::after {
      content: ""; position: absolute; inset: 10%; border-radius: 50%;
      background: radial-gradient(circle at 60% 40%, rgba(255,255,255,0.25), transparent 40%);
      filter: blur(10px);
    }

    /* Services */
    .section-title {
      font-family: "Space Grotesk", Inter, sans-serif; font-size: clamp(26px, 3vw, 38px);
      margin: 0 0 12px;
    }
    .section-subtitle { color: var(--muted); margin: 0 0 24px; }
    .cards {
      display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 18px;
    }
    .card {
      border-radius: 16px; padding: 18px; background: var(--card); border: 1px solid var(--border);
      box-shadow: var(--shadow); transition: transform .2s ease, box-shadow .2s ease;
      position: relative; overflow: hidden;
    }
    .card:hover { transform: translateY(-4px) scale(1.01); box-shadow: 0 18px 50px rgba(0,0,0,0.35); }
    .card .glow {
      position: absolute; inset: -40%; background: radial-gradient(circle at var(--mx,50%) var(--my,50%), rgba(122,162,255,0.18), transparent 40%);
      mix-blend-mode: screen; pointer-events: none; transition: opacity .2s ease; opacity: 0;
    }
    .card:hover .glow { opacity: 1; }
    .card h3 { margin: 8px 0 8px; font-size: 20px; }
    .badge {
      display: inline-block; padding: 4px 10px; border-radius: 999px; font-size: 12px; font-weight: 600;
      border: 1px solid var(--border); color: var(--muted); background: linear-gradient(180deg, var(--glass), transparent);
    }
    .chips { display: flex; flex-wrap: wrap; gap: 8px; margin: 12px 0; }
    .chip { padding: 6px 10px; border-radius: 999px; background: var(--glass); color: var(--text); border: 1px solid var(--border); font-size: 12px; }

    /* Builder */
    .builder {
      display: grid; grid-template-columns: 1.15fr 0.85fr; gap: 24px; align-items: start;
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.00));
      border: 1px solid var(--border); border-radius: 16px; padding: 18px; box-shadow: var(--shadow);
    }
    .field { display: grid; gap: 6px; margin-bottom: 12px; }
    label { font-size: 13px; color: var(--muted); }
    input[type="text"], textarea, select {
      width: 100%; padding: 12px 12px; border-radius: 10px; color: var(--text); background: var(--bg-2);
      border: 1px solid var(--border); outline: none; transition: border-color .15s ease, box-shadow .15s ease;
    }
    textarea { min-height: 130px; resize: vertical; }
    input:focus, textarea:focus, select:focus { border-color: var(--accent); box-shadow: 0 0 0 3px rgba(122,162,255,0.22); }

    .style-chips { display: flex; flex-wrap: wrap; gap: 8px; }
    .style-chip { padding: 8px 12px; border: 1px solid var(--border); background: var(--glass); border-radius: 999px; cursor: pointer; user-select: none; }
    .style-chip.active { background: linear-gradient(180deg, var(--accent), var(--accent-2)); color: #fff; border-color: transparent; }

    .preview {
      border: 1px solid var(--border); border-radius: 14px; background: #0b0f1a; padding: 16px; position: sticky; top: 90px;
      min-height: 260px; font-family: ui-monospace, SFMono-Regular, Menlo, Consolas, "Liberation Mono", monospace; line-height: 1.5;
      background-image: radial-gradient(600px 300px at 20% 0%, rgba(158,122,255,0.12), transparent 30%);
      white-space: pre-wrap;
    }
    .kbar { display: flex; gap: 8px; margin-top: 12px; flex-wrap: wrap; }
    .kbtn { padding: 8px 12px; border-radius: 8px; border: 1px solid var(--border); background: var(--card); color: var(--text); cursor: pointer; }
    .kbtn.primary { background: linear-gradient(180deg, var(--accent), var(--accent-2)); color: white; border: none; }

    /* Delivery */
    .delivery {
      display: grid; gap: 8px; border: 1px solid var(--border); border-radius: 14px; padding: 18px; background: var(--card);
    }
    .typewriter { font-family: ui-monospace, Menlo, Consolas, monospace; min-height: 52px; white-space: pre-wrap; }

    /* Socials, Gallery, Testimonials */
    .socials { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; }
    .social-card {
      padding: 16px; border-radius: 14px; border: 1px solid var(--border); background: linear-gradient(180deg, var(--card), transparent);
      display: flex; align-items: center; justify-content: center; gap: 10px; font-weight: 600; color: var(--text); text-decoration: none;
      box-shadow: var(--shadow);
    }
    .gallery {
      margin-top: 16px; display: grid; grid-template-columns: repeat(6, 1fr); gap: 8px;
    }
    .shot {
      aspect-ratio: 1/1; border: 1px solid var(--border); border-radius: 12px; overflow: hidden;
      background: radial-gradient(120px 120px at 60% 30%, rgba(122,162,255,0.25), transparent 60%), #0d1220;
      position: relative;
    }
    .shot img { width: 100%; height: 100%; object-fit: cover; display: block; }
    .shot::after {
      content: ""; position: absolute; inset: 0; background: linear-gradient(180deg, transparent, rgba(0,0,0,0.25));
    }

    /* FAQ / Trust */
    .faq { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; }
    .accordion { border: 1px solid var(--border); border-radius: 12px; background: var(--card); padding: 12px; }
    .accordion summary { cursor: pointer; list-style: none; font-weight: 600; }
    .accordion summary::-webkit-details-marker { display: none; }
    .badges { display: flex; gap: 10px; flex-wrap: wrap; }

    /* Footer */
    footer { padding: 32px 0; border-top: 1px solid var(--border); color: var(--muted); }
    .footer-grid { display: grid; grid-template-columns: 1fr auto; gap: 12px; align-items: center; }

    /* Responsive */
    @media (max-width: 980px) {
      .hero-grid, .builder, .faq { grid-template-columns: 1fr; }
      .cards { grid-template-columns: 1fr; }
      .socials { grid-template-columns: 1fr; }
      .gallery { grid-template-columns: repeat(3, 1fr); }
      .orb { width: 320px; height: 320px; margin: 0 auto; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="brand-logo" aria-hidden="true"></div>
        <div>
          <div style="font-weight:700;">Cosmic Nexus</div>
          <div style="font-size:12px; color:var(--muted)">Engineered by Ishan</div>
        </div>
      </div>
      <nav class="nav-links" aria-label="Primary">
        <a href="#services">Services</a>
        <a href="#builder">Create</a>
        <a href="#delivery">Deliver</a>
        <a href="#work">Work</a>
        <a href="#faq">FAQ</a>
        <button class="theme-toggle" id="themeToggle" aria-label="Toggle dark/light mode">🌙 <span>Theme</span></button>
        <button class="btn primary" onclick="scrollToId('builder')">Start Creating</button>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero" id="hero" aria-label="Welcome">
    <div class="galaxy"></div>
    <div class="container hero-grid">
      <div>
        <h1>Where Infinite Ideas Meet Perfect Execution</h1>
        <p>Transform your ideas into polished, ready‑to‑use outputs—prompts, scripts, thumbnails, SEO—guided by Ishan’s creative direction and precision.</p>
        <div class="cta-row">
          <button class="btn primary" onclick="scrollToId('builder')">Start Creating</button>
          <a class="btn" id="watchWorkBtn" href="#" target="_blank" rel="noopener">Watch My Work</a>
        </div>
        <div class="chips" style="margin-top:14px;">
          <span class="badge">Clear plan delivery</span>
          <span class="badge">Personal creative style</span>
          <span class="badge">Direct connection</span>
        </div>
      </div>
      <div>
        <div class="orb" role="img" aria-label="Animated cosmic orb"></div>
      </div>
    </div>
  </section>

  <!-- Services -->
  <section id="services" aria-label="Service Selection">
    <div class="container">
      <h2 class="section-title">Choose Your Creative Engine</h2>
      <p class="section-subtitle">Interactive, 3D‑hover cards with presets and deep options.</p>
      <div class="cards" id="serviceCards">
        <!-- Cards injected by JS -->
      </div>
    </div>
  </section>

  <!-- Builder -->
  <section id="builder" aria-label="Guided Input Form">
    <div class="container builder">
      <div>
        <h2 class="section-title">Guided Builder</h2>
        <p class="section-subtitle">Describe your idea; get a production‑ready prompt or plan with live preview.</p>

        <div class="field">
          <label for="topic">Topic / Idea</label>
          <input id="topic" type="text" placeholder="e.g., Epic anime fight sequence in a neon city" />
        </div>

        <div class="field">
          <label for="mood">Mood</label>
          <select id="mood">
            <option>Dynamic</option>
            <option>Cinematic</option>
            <option>Dreamy</option>
            <option>Dark</option>
            <option>Upbeat</option>
          </select>
        </div>

        <div class="field">
          <label for="audience">Audience</label>
          <input id="audience" type="text" placeholder="e.g., Anime fans 16–30" />
        </div>

        <div class="field">
          <label>Style Presets</label>
          <div class="style-chips" id="styleChips"></div>
        </div>

        <div class="field">
          <label for="details">Extra Details</label>
          <textarea id="details" placeholder="Key beats, references, pacing, camera moves, color palette..."></textarea>
        </div>

        <div class="kbar">
          <button class="kbtn" onclick="injectPreset()">Try Example</button>
          <button class="kbtn" onclick="clearBuilder()">Clear</button>
          <button class="kbtn primary" onclick="generate()">Generate Plan</button>
        </div>
      </div>

      <aside>
        <h3 style="margin:0 0 8px;">Live Preview</h3>
        <div id="preview" class="preview" aria-live="polite"></div>
        <div class="kbar">
          <button class="kbtn" onclick="copyPreview()">Copy</button>
          <button class="kbtn" onclick="downloadTxt()">Download TXT</button>
          <button class="kbtn" onclick="exportPDF()">Export PDF</button>
          <button class="kbtn" onclick="shareLink()">Get Share Link</button>
        </div>
      </aside>
    </div>
  </section>

  <!-- Delivery -->
  <section id="delivery" aria-label="Prompt/Plan Delivery">
    <div class="container delivery">
      <h2 class="section-title">Delivery & Handoff</h2>
      <p class="section-subtitle">Typewriter reveal, one‑click copy, and send to Ishan for review.</p>
      <div id="typewriter" class="typewriter"></div>
      <div class="kbar">
        <button class="kbtn" onclick="typeOut()">Reveal Again</button>
        <button class="kbtn primary" onclick="openReview()">Send to Ishan for Review</button>
      </div>
    </div>
  </section>

  <!-- Work / Socials -->
  <section id="work" aria-label="Connect & Learn More">
    <div class="container">
      <h2 class="section-title">Connect & Explore</h2>
      <p class="section-subtitle">Follow, watch, and browse highlights from the cosmos.</p>
      <div class="socials">
        <a class="social-card" id="ytLink" href="#" target="_blank" rel="noopener">📺 YouTube: Anime by Ishan</a>
        <a class="social-card" id="igLink" href="#" target="_blank" rel="noopener">📸 Instagram: @yourhandle</a>
        <a class="social-card" id="twLink" href="#" target="_blank" rel="noopener">🐦 X/Twitter: @optional</a>
      </div>
      <div class="gallery" id="gallery">
        <!-- Thumbnails injected -->
      </div>
      <div class="chips" style="margin-top:14px;">
        <span class="badge">Testimonials coming soon</span>
        <span class="badge">Rotating showcase</span>
      </div>
    </div>
  </section>

  <!-- FAQ / Trust -->
  <section id="faq" aria-label="Trust & Professionalism">
    <div class="container">
      <h2 class="section-title">Questions & Assurances</h2>
      <p class="section-subtitle">Transparent process, timelines, and rights.</p>
      <div class="faq">
        <details class="accordion">
          <summary>What do I get when I click Generate?</summary>
          <div>You'll receive a structured, ready‑to‑use prompt or production plan tailored to your inputs, including style, beats, and output settings.</div>
        </details>
        <details class="accordion">
          <summary>Can I request a manual review?</summary>
          <div>Yes—use “Send to Ishan for Review” to submit your plan with contact info for personalized feedback and refinement.</div>
        </details>
        <details class="accordion">
          <summary>Do I own the outputs?</summary>
          <div>You own the prompts and plans generated here; credits for collaborations are appreciated. For commissioned assets, terms are provided upon request.</div>
        </details>
        <details class="accordion">
          <summary>How fast is delivery?</summary>
          <div>Instant for auto‑generated plans; 24–72 hours for manual reviews depending on scope and queue.</div>
        </details>
      </div>
      <div class="badges" style="margin-top:14px;">
        <span class="badge">Performance optimized</span>
        <span class="badge">Accessible</span>
        <span class="badge">Responsive</span>
        <span class="badge">SEO‑ready</span>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer role="contentinfo">
    <div class="container footer-grid">
      <div>© <span id="year"></span> Cosmic Nexus. Made by Ishan.</div>
      <div class="chips">
        <span class="badge">Dark/Light</span>
        <span class="badge">Easter eggs</span>
        <span class="badge">Smooth transitions</span>
      </div>
    </div>
  </footer>

  <!-- Review Modal -->
  <dialog id="reviewModal" style="border:none; border-radius:16px; padding:0; max-width:560px; width:90%; background:var(--bg); color:var(--text);">
    <form method="dialog" style="padding:18px;">
      <h3 style="margin:0 0 8px;">Send to Ishan for Review</h3>
      <p class="section-subtitle" style="margin-top:0;">Share your plan and contact details for personalized feedback.</p>
      <div class="field">
        <label for="name">Name</label>
        <input id="name" type="text" placeholder="Your name" required />
      </div>
      <div class="field">
        <label for="email">Email</label>
        <input id="email" type="text" placeholder="name@email.com" required />
      </div>
      <div class="field">
        <label for="message">Message</label>
        <textarea id="message" placeholder="Context, goals, deadlines…"></textarea>
      </div>
      <div class="kbar">
        <button class="kbtn" value="cancel">Cancel</button>
        <button class="kbtn primary" value="submit" onclick="submitReview(event)">Send</button>
      </div>
    </form>
  </dialog>

  <script>
    // -------- Config: Replace these with real links/handles --------
    const CONFIG = {
      links: {
        youtube: "https://youtube.com/@AnimeByIshan",
        instagram: "https://instagram.com/yourhandle",
        twitter: "https://twitter.com/optional",
        watchWork: "https://youtube.com/@AnimeByIshan"
      },
      gallery: [
        // Replace with your thumbnails/screenshots
        "https://images.unsplash.com/photo-1549880338-65ddcdfd017b?q=80&w=800&auto=format&fit=crop",
        "https://images.unsplash.com/photo-1517697471339-4aa32003c11a?q=80&w=800&auto=format&fit=crop",
        "https://images.unsplash.com/photo-1495567720989-cebdbdd97913?q=80&w=800&auto=format&fit=crop",
        "https://images.unsplash.com/photo-1520975682031-ae5b3a1e7c5a?q=80&w=800&auto=format&fit=crop",
        "https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?q=80&w=800&auto=format&fit=crop",
        "https://images.unsplash.com/photo-1535223289827-42f1e9919769?q=80&w=800&auto=format&fit=crop"
      ]
    };

    // -------- Utilities --------
    function scrollToId(id) { document.getElementById(id)?.scrollIntoView({ behavior: 'smooth', block: 'start' }); }
    function setTheme(mode) { document.documentElement.setAttribute('data-theme', mode); localStorage.setItem('theme', mode); }
    function toggleTheme() { const cur = document.documentElement.getAttribute('data-theme') || 'dark'; setTheme(cur === 'dark' ? 'light' : 'dark'); }
    document.getElementById('themeToggle').addEventListener('click', toggleTheme);
    (function initTheme(){ const saved = localStorage.getItem('theme') || 'dark'; setTheme(saved); })();

    // Header links
    document.getElementById('ytLink').href = CONFIG.links.youtube;
    document.getElementById('igLink').href = CONFIG.links.instagram;
    document.getElementById('twLink').href = CONFIG.links.twitter;
    document.getElementById('watchWorkBtn').href = CONFIG.links.watchWork;

    // Year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Easter eggs: hover stars
    document.body.addEventListener('mousemove', (e) => {
      document.querySelectorAll('.card .glow').forEach(el => {
        el.style.setProperty('--mx', e.offsetX + 'px');
        el.style.setProperty('--my', e.offsetY + 'px');
      });
    });

    // Services Data
    const SERVICES = [
      {
        id: 'video',
        title: 'Text‑to‑Video Prompting',
        icon: '🎥',
        desc: 'Scene‑by‑scene prompts, camera moves, timing, and visual directives for cinematic AI video.',
        chips: ['Cinematic', 'Anime', 'Cyberpunk', 'Realistic', 'Dreamy'],
        badge: 'Pro'
      },
      {
        id: 'image',
        title: 'AI Image & Thumbnail Prompts',
        icon: '🖼️',
        desc: 'High‑CTR thumbnail prompt packs with composition, typography, lighting, and brand style.',
        chips: ['Bold', 'Minimal', 'Vibrant', 'Moody', 'Studio']
      },
      {
        id: 'script',
        title: 'YouTube Script & SEO Packs',
        icon: '📝',
        desc: 'Hook, structure, pacing, retention beats, title/description/tags, and upload checklist.',
        chips: ['Explainer', 'Narrative', 'Tutorial', 'Review', 'Shorts'],
        badge: 'New'
      }
    ];

    // Styles
    const STYLE_PRESETS = ['cinematic','anime','cyberpunk','realistic','dreamy','studio','moody','lofi','vintage','surreal'];

    // Inject service cards
    const cardsWrap = document.getElementById('serviceCards');
    SERVICES.forEach(s => {
      const el = document.createElement('div');
      el.className = 'card';
      el.innerHTML = `
        <div class="glow"></div>
        <div style="display:flex; align-items:center; justify-content:space-between;">
          <div class="badge">${s.badge || 'Featured'}</div>
          <button class="kbtn" onclick="selectService('${s.id}')">Select</button>
        </div>
        <h3>${s.icon} ${s.title}</h3>
        <div style="color:var(--muted); font-size:14px;">${s.desc}</div>
        <div class="chips">${s.chips.map(c => `<span class="chip">${c}</span>`).join('')}</div>
      `;
      cardsWrap.appendChild(el);
    });

    // Inject style chips
    const chipsWrap = document.getElementById('styleChips');
    const activeStyles = new Set();
    STYLE_PRESETS.forEach(p => {
      const c = document.createElement('button');
      c.type = 'button';
      c.className = 'style-chip';
      c.textContent = p;
      c.setAttribute('aria-pressed', 'false');
      c.addEventListener('click', () => {
        const on = c.classList.toggle('active');
        c.setAttribute('aria-pressed', String(on));
        on ? activeStyles.add(p) : activeStyles.delete(p);
        updatePreview();
      });
      chipsWrap.appendChild(c);
    });

    // Builder inputs
    const topicEl = document.getElementById('topic');
    const moodEl = document.getElementById('mood');
    const audienceEl = document.getElementById('audience');
    const detailsEl = document.getElementById('details');
    [topicEl, moodEl, audienceEl, detailsEl].forEach(el => el.addEventListener('input', updatePreview));

    let selectedService = 'video';
    function selectService(id) { selectedService = id; scrollToId('builder'); updatePreview(); }

    function injectPreset() {
      topicEl.value = "Epic anime duel on a neon‑drenched rooftop during a thunderstorm";
      moodEl.value = "Cinematic";
      audienceEl.value = "Anime and action fans 16–30";
      detailsEl.value = "Wide establishing shot, dolly push‑in, electric purple/teal palette, slow‑mo clash, sparks, rain droplets, final hero shot on edge.";
      document.querySelectorAll('.style-chip').forEach((btn, i) => {
        if (['anime','cyberpunk','cinematic','realistic'].includes(btn.textContent)) {
          btn.classList.add('active'); btn.setAttribute('aria-pressed','true'); activeStyles.add(btn.textContent);
        }
      });
      updatePreview();
    }

    function clearBuilder() {
      topicEl.value = ""; audienceEl.value = ""; detailsEl.value = "";
      moodEl.value = "Dynamic";
      activeStyles.clear();
      document.querySelectorAll('.style-chip').forEach(btn => { btn.classList.remove('active'); btn.setAttribute('aria-pressed','false'); });
      updatePreview();
    }

    function buildPrompt() {
      const topic = topicEl.value.trim();
      const mood = moodEl.value.trim();
      const audience = audienceEl.value.trim();
      const details = detailsEl.value.trim();
      const styles = Array.from(activeStyles);

      const opening = `Project: ${selectedService.toUpperCase()} • Mood: ${mood} • Styles: ${styles.join(", ") || "default"}`;
      const core = topic ? `Topic: ${topic}` : "Topic: (add your idea)";
      const aud = audience ? `Audience: ${audience}` : "";
      const extra = details ? `Notes: ${details}` : "";

      if (selectedService === 'video') {
        return `${opening}

${core}
${aud}
${extra}

Deliver:
- Shot list with camera/lens and movement.
- Timing per beat (sec).
- Color/lighting and FX guidance.
- Aspect ratio(s) and model hints.
- Export settings.`;
      } else if (selectedService === 'image') {
        return `${opening}

${core}
${aud}
${extra}

Deliver:
- Thumbnail composition (rule of thirds, focal point).
- Typography prompt with font vibe.
- Lighting/color palette and contrast strategy.
- Variations (3).
- Export sizes (16:9, 9:16, 1:1).`;
      } else {
        return `${opening}

${core}
${aud}
${extra}

Deliver:
- Hook (first 5 seconds).
- Outline with retention beats and timestamps.
- Script body with pacing notes.
- Title, description, tags, and end screen plan.
- Upload checklist.`;
      }
    }

    function updatePreview() {
      const text = buildPrompt();
      document.getElementById('preview').textContent = text;
    }
    updatePreview();

    // Actions
    async function copyPreview() {
      const text = document.getElementById('preview').textContent.trim();
      if (!text) return;
      await navigator.clipboard.writeText(text);
      toast('Copied!');
    }

    function downloadTxt() {
      const text = document.getElementById('preview').textContent.trim();
      const blob = new Blob([text], { type: 'text/plain' });
      const url = URL.createObjectURL(blob);
      const a = Object.assign(document.createElement('a'), { href: url, download: 'cosmic-plan.txt' });
      document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
    }

    function exportPDF() {
      // Simple print-to-PDF; for advanced control integrate jsPDF later
      window.print();
    }

    function shareLink() {
      const params = new URLSearchParams({
        s: selectedService,
        t: topicEl.value,
        m: moodEl.value,
        a: audienceEl.value,
        d: detailsEl.value,
        st: Array.from(activeStyles).join(',')
      });
      const link = `${location.origin}${location.pathname}?${params.toString()}`;
      navigator.clipboard.writeText(link);
      toast('Share link copied!');
    }

    // Prefill from URL
    (function prefillFromUrl(){
      const q = new URLSearchParams(location.search);
      if (!q.size) return;
      selectedService = q.get('s') || selectedService;
      topicEl.value = q.get('t') || topicEl.value;
      moodEl.value = q.get('m') || moodEl.value;
      audienceEl.value = q.get('a') || audienceEl.value;
      detailsEl.value = q.get('d') || detailsEl.value;
      const st = (q.get('st') || "").split(',').filter(Boolean);
      document.querySelectorAll('.style-chip').forEach(btn => {
        if (st.includes(btn.textContent)) { btn.classList.add('active'); btn.setAttribute('aria-pressed','true'); activeStyles.add(btn.textContent); }
      });
      updatePreview();
    })();

    // Typewriter delivery
    let typerTimer;
    function typeOut() {
      const text = document.getElementById('preview').textContent;
      const out = document.getElementById('typewriter');
      out.textContent = '';
      let i = 0;
      clearInterval(typerTimer);
      typerTimer = setInterval(() => {
        out.textContent += text[i] || '';
        i++;
        if (i >= text.length) clearInterval(typerTimer);
      }, 12);
      scrollToId('delivery');
    }
    // Auto type on generate
    function generate(){ updatePreview(); typeOut(); }

    // Review Modal
    const reviewModal = document.getElementById('reviewModal');
    function openReview(){ reviewModal.showModal(); }
    function submitReview(e){
      e.preventDefault();
      const payload = {
        name: document.getElementById('name').value.trim(),
        email: document.getElementById('email').value.trim(),
        message: document.getElementById('message').value.trim(),
        plan: document.getElementById('preview').textContent.trim(),
        service: selectedService,
        timestamp: new Date().toISOString()
      };
      console.log('Review request:', payload);
      reviewModal.close();
      toast('Sent to Ishan! Check console for payload.');
      // TODO: Integrate real endpoint or email via serverless function
    }

    // Gallery
    const galleryWrap = document.getElementById('gallery');
    CONFIG.gallery.forEach(src => {
      const el = document.createElement('div');
      el.className = 'shot';
      el.innerHTML = `<img src="${src}" alt="Work sample">`;
      galleryWrap.appendChild(el);
    });

    // Social link setup
    function setSocials(){
      document.getElementById('ytLink').href = CONFIG.links.youtube;
      document.getElementById('igLink').href = CONFIG.links.instagram;
      document.getElementById('twLink').href = CONFIG.links.twitter;
      document.getElementById('watchWorkBtn').href = CONFIG.links.watchWork;
    }
    setSocials();

    // Toast
    function toast(msg) {
      const t = document.createElement('div');
      t.textContent = msg;
      t.style.cssText = `
        position: fixed; bottom: 18px; left: 50%; transform: translateX(-50%);
        background: linear-gradient(180deg, var(--glass), transparent);
        border: 1px solid var(--border); color: var(--text);
        padding: 10px 14px; border-radius: 10px; z-index: 1000; box-shadow: var(--shadow);
      `;
      document.body.appendChild(t);
      setTimeout(() => t.remove(), 1600);
    }

    // Smooth section transitions
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) entry.target.animate([{opacity:0, transform:'translateY(8px)'},{opacity:1, transform:'translateY(0)'}], { duration: 500, fill: 'forwards', easing: 'ease-out' });
      });
    }, { threshold: 0.08 });
    document.querySelectorAll('section').forEach(s => observer.observe(s));
  </script>
</body>
</html>
