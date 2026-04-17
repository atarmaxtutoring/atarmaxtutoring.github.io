# atarmaxtutoring.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Private Tutoring</title>
  <style>
    :root {
      --bg: #f7f8fc;
      --surface: #ffffff;
      --text: #18212f;
      --muted: #5f6b7a;
      --line: #dfe5ee;
      --accent: #2457d6;
      --accent-2: #eef3ff;
      --radius: 18px;
      --shadow: 0 10px 30px rgba(24, 33, 47, 0.08);
      --max: 1120px;
    }

    * { box-sizing: border-box; }
    html { scroll-behaviour: smooth; }
    body {
      margin: 0;
      font-family: Inter, Arial, Helvetica, sans-serif;
      background: linear-gradient(180deg, #f9fbff 0%, #f5f7fb 100%);
      colour: var(--text);
      line-height: 1.55;
    }

    a { colour: inherit; text-decoration: none; }

    .container {
      width: min(calc(100% - 32px), var(--max));
      margin: 0 auto;
    }

    .nav {
      position: sticky;
      top: 0;
      z-index: 10;
      backdrop-filter: blur(10px);
      background: rgba(247, 248, 252, 0.82);
      border-bottom: 1px solid rgba(223, 229, 238, 0.8);
    }

    .nav-inner {
      display: flex;
      align-items: centre;
      justify-content: space-between;
      padding: 16px 0;
      gap: 20px;
    }

    .brand {
      font-size: 1.05rem;
      font-weight: 800;
      letter-spacing: 0.01em;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      colour: var(--muted);
      font-size: 0.95rem;
    }

    .hero {
      padding: 72px 0 42px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.15fr 0.85fr;
      gap: 28px;
      align-items: centre;
    }

    .eyebrow {
      display: inline-flex;
      padding: 8px 12px;
      border-radius: 999px;
      background: var(--accent-2);
      colour: var(--accent);
      font-size: 0.9rem;
      font-weight: 700;
      margin-bottom: 16px;
    }

    h1, h2, h3, p { margin-top: 0; }

    h1 {
      font-size: clamp(2.2rem, 4vw, 4.2rem);
      line-height: 1.05;
      letter-spacing: -0.03em;
      margin-bottom: 18px;
    }

    .lead {
      font-size: 1.08rem;
      colour: var(--muted);
      max-width: 62ch;
      margin-bottom: 24px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-bottom: 18px;
    }

    .btn {
      display: inline-flex;
      align-items: centre;
      justify-content: centre;
      padding: 13px 18px;
      border-radius: 12px;
      font-weight: 700;
      border: 1px solid transparent;
      transition: transform 0.18s ease, box-shadow 0.18s ease, background 0.18s ease;
      cursor: pointer;
    }

    .btn:hover { transform: translateY(-1px); }

    .btn-primary {
      background: var(--accent);
      colour: white;
      box-shadow: 0 10px 24px rgba(36, 87, 214, 0.22);
    }

    .btn-secondary {
      background: white;
      border-colour: var(--line);
      colour: var(--text);
    }

    .hero-card,
    .card {
      background: var(--surface);
      border: 1px solid rgba(223, 229, 238, 0.95);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }

    .hero-card {
      padding: 24px;
    }

    .mini-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 14px;
      margin-top: 16px;
    }

    .stat {
      background: #fbfcff;
      border: 1px solid var(--line);
      border-radius: 14px;
      padding: 16px;
    }

    .stat strong {
      display: block;
      font-size: 1.05rem;
      margin-bottom: 4px;
    }

    .stat span {
      colour: var(--muted);
      font-size: 0.92rem;
    }

    .section {
      padding: 28px 0;
    }

    .section-title {
      font-size: clamp(1.6rem, 2.4vw, 2.35rem);
      margin-bottom: 10px;
      letter-spacing: -0.02em;
    }

    .section-copy {
      colour: var(--muted);
      max-width: 68ch;
      margin-bottom: 22px;
    }

    .three-up,
    .two-up {
      display: grid;
      gap: 18px;
    }

    .three-up { grid-template-columns: repeat(3, 1fr); }
    .two-up { grid-template-columns: repeat(2, 1fr); }

    .card {
      padding: 22px;
    }

    .card h3 {
      margin-bottom: 10px;
      font-size: 1.1rem;
    }

    .card p,
    .card li,
    .muted {
      colour: var(--muted);
    }

    ul.clean {
      margin: 0;
      padding-left: 18px;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 0.85fr 1.15fr;
      gap: 20px;
      align-items: start;
    }

    .contact-card {
      padding: 24px;
    }

    form {
      display: grid;
      gap: 14px;
    }

    label {
      display: grid;
      gap: 7px;
      font-weight: 700;
      font-size: 0.95rem;
    }

    input, textarea, select {
      width: 100%;
      padding: 14px 14px;
      border-radius: 12px;
      border: 1px solid var(--line);
      font: inherit;
      colour: var(--text);
      background: white;
    }

    textarea { min-height: 140px; resize: vertical; }

    .small {
      font-size: 0.88rem;
      colour: var(--muted);
    }

    .footer {
      padding: 28px 0 50px;
      colour: var(--muted);
      font-size: 0.92rem;
    }

    @media (max-width: 920px) {
      .hero-grid,
      .contact-grid,
      .three-up,
      .two-up {
        grid-template-columns: 1fr;
      }

      .nav-inner {
        flex-direction: column;
        align-items: flex-start;
      }
    }
  </style>
</head>
<body>
  <nav class="nav">
    <div class="container nav-inner">
      <div class="brand">Private Tutoring</div>
      <div class="nav-links">
        <a href="#services">Services</a>
        <a href="#why">Why Me</a>
        <a href="#process">How It Works</a>
        <a href="#contact">Enquire</a>
      </div>
    </div>
  </nav>

  <header class="hero">
    <div class="container hero-grid">
      <div>
        <div class="eyebrow">Years 7 to 12, personalised support</div>
        <h1>Clear, practical tutoring that helps students improve fast.</h1>
        <p class="lead">
          I offer tailored tutoring with a strong focus on confidence, structure, and results. Whether a student needs help with essay writing, textual analysis, or exam preparation, lessons are built around what they actually need.
        </p>
        <div class="actions">
          <a class="btn btn-primary" href="#contact">Book an enquiry</a>
          <a class="btn btn-secondary" href="#services">See subjects</a>
        </div>
        <p class="small">Online and in-person options available. Update this line with your suburb, availability, and preferred lesson format.</p>
      </div>

      <div class="hero-card">
        <h3>At a glance</h3>
        <p class="muted">Swap these details out for your real offer. Keep it brief and direct.</p>
        <div class="mini-grid">
          <div class="stat">
            <strong>English tutoring</strong>
            <span>Essay writing, analysis, exam prep</span>
          </div>
          <div class="stat">
            <strong>Senior support</strong>
            <span>Years 10 to 12 and HSC guidance</span>
          </div>
          <div class="stat">
            <strong>Structured lessons</strong>
            <span>Resources, feedback, and clear goals</span>
          </div>
          <div class="stat">
            <strong>Flexible delivery</strong>
            <span>Online or local in-person sessions</span>
          </div>
        </div>
      </div>
    </div>
  </header>

  <section class="section" id="services">
    <div class="container">
      <h2 class="section-title">Services</h2>
      <p class="section-copy">This section should match exactly what you want people to enquire about. The easier it is to understand, the more likely people are to message you.</p>
      <div class="three-up">
        <article class="card">
          <h3>Junior English</h3>
          <p>Reading comprehension, paragraph structure, essay writing, grammar support, and confidence building for Years 7 to 9.</p>
        </article>
        <article class="card">
          <h3>Senior English</h3>
          <p>Module support, close analysis, thesis building, practice responses, and exam strategy for Years 10 to 12.</p>
        </article>
        <article class="card">
          <h3>School assessment support</h3>
          <p>Help with drafts, feedback, planning, and refining written responses in a way that improves both marks and understanding.</p>
        </article>
      </div>
    </div>
  </section>

  <section class="section" id="why">
    <div class="container">
      <h2 class="section-title">Why families choose this tutoring</h2>
      <p class="section-copy">Parents usually want three things, clarity, trust, and evidence that you know what you are doing. This section should do that work for you.</p>
      <div class="two-up">
        <article class="card">
          <h3>What students get</h3>
          <ul class="clean">
            <li>Lessons tailored to the student’s current level</li>
            <li>Simple explanations that make difficult content manageable</li>
            <li>Clear feedback on writing and how to improve it</li>
            <li>Consistent routines that build confidence over time</li>
          </ul>
        </article>
        <article class="card">
          <h3>What parents value</h3>
          <ul class="clean">
            <li>Professional communication and organised lessons</li>
            <li>A focus on genuine improvement, not just rushing homework</li>
            <li>Useful resources students can revisit between sessions</li>
            <li>A calm, supportive approach that keeps students engaged</li>
          </ul>
        </article>
      </div>
    </div>
  </section>

  <section class="section" id="process">
    <div class="container">
      <h2 class="section-title">How it works</h2>
      <p class="section-copy">Make the next step feel effortless. Most people will enquire if the process feels simple and low-pressure.</p>
      <div class="three-up">
        <article class="card">
          <h3>1. Enquiry</h3>
          <p>Parents fill in the short form with the student’s year level, subject, and what help they need.</p>
        </article>
        <article class="card">
          <h3>2. Quick reply</h3>
          <p>You respond by email, confirm availability, and organise a first lesson or phone call.</p>
        </article>
        <article class="card">
          <h3>3. First session</h3>
          <p>The first lesson identifies strengths, gaps, and the best way to move forward.</p>
        </article>
      </div>
    </div>
  </section>

  <section class="section" id="contact">
    <div class="container contact-grid">
      <div class="card contact-card">
        <h2 class="section-title" style="font-size: 1.8rem; margin-bottom: 12px;">Enquire now</h2>
        <p class="section-copy" style="margin-bottom: 16px;">
          This form is set up for Formspree. Replace the action link with your own Formspree endpoint and submissions will be sent to your email.
        </p>
        <p class="small">
          You can also replace the form with a simple mailto link if you want the absolute easiest option, but a real form usually converts better.
        </p>
      </div>

      <div class="card contact-card">
        <form action="https://formspree.io/f/your-form-id" method="POST">
          <label>
            Parent or student name
            <input type="text" name="name" placeholder="Your name" required />
          </label>

          <label>
            Email address
            <input type="email" name="email" placeholder="you@example.com" required />
          </label>

          <label>
            Year level
            <select name="year_level" required>
              <option value="">Select a year</option>
              <option>Year 7</option>
              <option>Year 8</option>
              <option>Year 9</option>
              <option>Year 10</option>
              <option>Year 11</option>
              <option>Year 12</option>
            </select>
          </label>

          <label>
            Subject or support needed
            <input type="text" name="subject" placeholder="English, essay writing, exam prep, etc." required />
          </label>

          <label>
            Message
            <textarea name="message" placeholder="Tell me what support you are looking for" required></textarea>
          </label>

          <button class="btn btn-primary" type="submit">Send enquiry</button>
        </form>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="container">
      Add your name, suburb, contact email, rates, and available days here. You can also add one short testimonial once you have permission to use it.
    </div>
  </footer>
</body>
</html>
