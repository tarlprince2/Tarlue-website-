<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Custom sports jerseys, team kits, and athletic apparel. Message Tarlue Sports on WhatsApp to order." />
  <title>Tarlue Sports | Custom Jerseys</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700;800&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg: #f4f1eb;
      --white: #ffffff;
      --paper: #f9f6f1;
      --text: #141414;
      --muted: #676660;
      --line: #ddd6cc;
      --gold: #caa76d;
      --gold-dark: #876839;
      --dark: #171a1d;
      --whatsapp: #25d366;
    }

    * { box-sizing: border-box; }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: "DM Sans", Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    img { max-width: 100%; display: block; }
    a { color: inherit; text-decoration: none; }

    .container {
      width: min(1180px, calc(100% - 34px));
      margin: 0 auto;
    }

    .topbar {
      background: var(--dark);
      color: var(--white);
      text-align: center;
      font-size: 10px;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      padding: 9px 10px;
      font-weight: 700;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 20;
      background: rgba(244, 241, 235, 0.96);
      border-bottom: 1px solid var(--line);
      backdrop-filter: blur(8px);
    }

    .nav {
      min-height: 78px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 18px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      font-size: 18px;
      flex-shrink: 0;
    }

    .brand-mark {
      width: 46px;
      height: 30px;
      display: block;
      flex-shrink: 0;
      color: #111;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 28px;
    }

    .nav-links a {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: #4a4a46;
    }

    .nav-links a:hover { color: var(--gold-dark); }

    .header-btn,
    .btn {
      display: inline-flex;
      min-height: 46px;
      align-items: center;
      justify-content: center;
      padding: 0 18px;
      background: var(--gold);
      border: 1px solid var(--gold);
      color: #111;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 10px;
      font-weight: 800;
      transition: transform 0.2s ease, background 0.2s ease;
    }

    .header-btn:hover,
    .btn:hover {
      transform: translateY(-2px);
      background: #d9b57c;
    }

    .hero {
      min-height: 640px;
      display: flex;
      align-items: center;
      position: relative;
      overflow: hidden;
      background:
        linear-gradient(90deg, rgba(244,241,235,0.96) 0%, rgba(244,241,235,0.82) 38%, rgba(244,241,235,0.2) 100%),
        url("https://images.unsplash.com/photo-1517466787929-bc90951d0974?auto=format&fit=crop&w=1800&q=80") center/cover no-repeat;
    }

    .hero-inner {
      width: min(650px, 90%);
      margin-left: max(5%, calc((100vw - 1180px) / 2));
      padding: 70px 0;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 12px;
      color: var(--gold-dark);
      font-size: 10px;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      font-weight: 800;
    }

    .eyebrow::before {
      content: "";
      width: 24px;
      height: 1px;
      background: currentColor;
      display: block;
    }

    .hero h1 {
      margin: 18px 0 16px;
      font-size: clamp(3.7rem, 8vw, 8.5rem);
      line-height: 0.84;
      letter-spacing: -0.08em;
      text-transform: uppercase;
      font-weight: 800;
    }

    .hero h1 span {
      color: var(--gold-dark);
    }

    .hero p {
      max-width: 480px;
      color: var(--muted);
      font-size: 16px;
      margin: 0 0 26px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    .button-outline {
      display: inline-flex;
      min-height: 46px;
      align-items: center;
      justify-content: center;
      padding: 0 18px;
      border: 1px solid var(--text);
      color: var(--text);
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 10px;
      font-weight: 800;
      background: transparent;
      transition: background 0.2s ease, color 0.2s ease;
    }

    .button-outline:hover {
      background: var(--text);
      color: var(--white);
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      border-top: 1px solid var(--line);
      border-bottom: 1px solid var(--line);
      background: rgba(255,255,255,0.25);
    }

    .stat {
      border-right: 1px solid var(--line);
      text-align: center;
      padding: 24px 14px;
    }

    .stat:last-child { border-right: 0; }

    .stat strong {
      display: block;
      margin-bottom: 5px;
      font-size: 21px;
      letter-spacing: -0.04em;
      font-weight: 800;
    }

    .stat span {
      font-size: 10px;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .section {
      padding: 88px 0;
    }

    .section-head {
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      gap: 20px;
      margin-bottom: 24px;
    }

    .section-head h2 {
      margin: 10px 0 0;
      font-size: clamp(2.5rem, 5vw, 4.6rem);
      letter-spacing: -0.07em;
      line-height: 0.9;
      text-transform: uppercase;
      font-weight: 800;
    }

    .link-text {
      border-bottom: 1px solid var(--gold-dark);
      color: var(--gold-dark);
      padding-bottom: 4px;
      font-size: 10px;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      font-weight: 800;
      white-space: nowrap;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 18px;
    }

    .product-card {
      background: var(--white);
      border: 1px solid var(--line);
      overflow: hidden;
      transition: transform 0.2s ease, border-color 0.2s ease;
    }

    .product-card:hover {
      transform: translateY(-3px);
      border-color: rgba(202,167,109,0.7);
    }

    .product-img {
      position: relative;
      aspect-ratio: 4 / 5;
      overflow: hidden;
      background: #ece5dc;
    }

    .product-img img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.4s ease;
    }

    .product-card:hover .product-img img { transform: scale(1.04); }

    .badge {
      position: absolute;
      top: 12px;
      left: 12px;
      background: var(--gold);
      color: #111;
      font-size: 9px;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      font-weight: 800;
      padding: 7px 8px;
    }

    .product-body {
      padding: 15px 14px 18px;
    }

    .product-meta {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      margin-bottom: 6px;
    }

    .product-meta h3 {
      margin: 0;
      font-size: 14px;
      text-transform: uppercase;
      letter-spacing: -0.02em;
    }

    .price {
      font-size: 14px;
      font-weight: 800;
      color: var(--gold-dark);
      white-space: nowrap;
    }

    .product-body p {
      margin: 0 0 16px;
      font-size: 11px;
      letter-spacing: 0.08em;
      color: var(--muted);
      text-transform: uppercase;
    }

    .product-order {
      display: flex;
      width: 100%;
      min-height: 40px;
      align-items: center;
      justify-content: center;
      border: 1px solid var(--text);
      background: transparent;
      color: var(--text);
      text-transform: uppercase;
      letter-spacing: 0.11em;
      font-size: 9px;
      font-weight: 800;
      transition: background 0.2s ease, color 0.2s ease;
    }

    .product-order:hover {
      background: var(--text);
      color: var(--white);
    }

    .aboutsec {
      background: var(--white);
      border-top: 1px solid var(--line);
      border-bottom: 1px solid var(--line);
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      align-items: center;
      gap: 32px;
      padding: 88px 0;
    }

    .about-copy h2, .team-copy h2 {
      margin: 12px 0 18px;
      font-size: clamp(2.5rem, 5vw, 4.5rem);
      letter-spacing: -0.07em;
      line-height: 0.9;
      text-transform: uppercase;
      font-weight: 800;
    }

    .about-copy p, .team-copy p {
      max-width: 520px;
      color: var(--muted);
      margin: 0 0 22px;
      font-size: 14px;
    }

    .steps {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }

    .step {
      padding: 18px 15px;
      border: 1px solid var(--line);
      background: var(--paper);
    }

    .step-number {
      width: 30px;
      height: 30px;
      display: grid;
      place-items: center;
      border-radius: 50%;
      background: var(--gold);
      font-weight: 800;
      font-size: 12px;
      margin-bottom: 12px;
    }

    .step h3 {
      margin: 0 0 6px;
      font-size: 12px;
      letter-spacing: 0.06em;
      text-transform: uppercase;
    }

    .step p {
      margin: 0;
      font-size: 11px;
      color: var(--muted);
      line-height: 1.6;
    }

    .about-image {
      min-height: 420px;
      background:
        linear-gradient(135deg, rgba(202,167,109,0.18), rgba(255,255,255,0.02)),
        url("https://images.unsplash.com/photo-1541099649105-f69ad21f3246?auto=format&fit=crop&w=1200&q=80") center/cover no-repeat;
      border: 1px solid var(--line);
    }

    .team-banner {
      background: var(--dark);
      color: var(--white);
      padding: 70px 0;
    }

    .team-grid {
      display: grid;
      grid-template-columns: 1.12fr 0.88fr;
      gap: 36px;
      align-items: center;
    }

    .team-copy .eyebrow { color: var(--gold); }
    .team-copy p { color: rgba(255,255,255,.72); }

    .team-mark {
      display: grid;
      place-items: center;
      min-height: 300px;
      border: 1px solid rgba(255,255,255,.20);
      font-size: clamp(100px, 16vw, 170px);
      font-weight: 800;
      letter-spacing: -0.12em;
      color: var(--gold);
    }

    .faq-list {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 14px;
    }

    .faq-item {
      padding: 20px 18px;
      border: 1px solid var(--line);
      background: rgba(255,255,255,0.4);
    }

    .faq-item h3 {
      margin: 0 0 8px;
      font-size: 13px;
      letter-spacing: -0.02em;
      text-transform: uppercase;
    }

    .faq-item p {
      margin: 0;
      font-size: 12px;
      color: var(--muted);
      line-height: 1.6;
    }

    .contact-strip {
      background: var(--gold);
      color: #111;
      padding: 20px 0;
    }

    .contact-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 18px;
      flex-wrap: wrap;
    }

    .contact-inner strong {
      font-size: 11px;
      letter-spacing: 0.14em;
      text-transform: uppercase;
    }

    .wa-btn {
      display: inline-flex;
      min-height: 42px;
      align-items: center;
      justify-content: center;
      padding: 0 15px;
      border: 1px solid rgba(17,17,17,0.6);
      color: #111;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 10px;
      font-weight: 800;
    }

    .wa-btn:hover {
      background: #111;
      color: white;
    }

    footer {
      background: #111;
      color: var(--white);
      padding: 26px 0 34px;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 22px;
      flex-wrap: wrap;
    }

    .footer-links {
      display: flex;
      flex-wrap: wrap;
      gap: 18px;
      font-size: 10px;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: #d8d7d3;
    }

    .copyright {
      font-size: 10px;
      color: #bdbcb6;
    }

    .whatsapp-float {
      position: fixed;
      right: 20px;
      bottom: 20px;
      width: 58px;
      height: 58px;
      display: grid;
      place-items: center;
      border-radius: 50%;
      background: var(--whatsapp);
      color: white;
      font-size: 28px;
      font-weight: 800;
      box-shadow: 0 12px 30px rgba(37,211,102,0.35);
      z-index: 30;
    }

    .whatsapp-float:hover {
      transform: translateY(-2px);
    }

    .menu-toggle {
      display: none;
      width: 42px;
      height: 42px;
      border: 1px solid var(--line);
      background: transparent;
      font-size: 22px;
      color: var(--text);
    }

    @media (max-width: 940px) {
      .products {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .about-grid, .team-grid {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 680px) {
      .nav-links {
        display: none;
        position: absolute;
        left: 0;
        right: 0;
        top: 78px;
        background: rgba(244,241,235,0.98);
        border-bottom: 1px solid var(--line);
        padding: 12px 17px 20px;
        flex-direction: column;
        align-items: flex-start;
      }

      .nav-links.open { display: flex; }

      .menu-toggle { display: block; }

      .header-btn { display: none; }

      .hero {
        min-height: 560px;
      }

      .hero-inner {
        margin-left: 5%;
      }

      .stats {
        grid-template-columns: 1fr;
      }

      .stat {
        border-right: 0;
        border-bottom: 1px solid var(--line);
      }

      .stat:last-child { border-bottom: 0; }

      .section-head {
        flex-direction: column;
        align-items: flex-start;
      }

      .products {
        grid-template-columns: 1fr;
      }

      .steps, .faq-list {
        grid-template-columns: 1fr;
      }

      .contact-inner {
        flex-direction: column;
        align-items: flex-start;
      }
    }
  </style>
</head>
<body>
  <div class="topbar">Custom team kits • WhatsApp orders • No online checkout</div>

  <header>
    <div class="container nav">
      <a href="#" class="brand" aria-label="Tarlue Sports Home">
        <svg class="brand-mark" viewBox="0 0 320 180" aria-hidden="true">
          <path fill="currentColor" d="M0 0H320L268 48L211 60V125L160 180L109 125V60L52 48L0 0ZM90 20L146 42V180H174V42L230 20H90Z" />
        </svg>
        <span>Tarlue Sports</span>
      </a>

      <nav class="nav-links" id="nav-links">
        <a href="#shop">Jerseys</a>
        <a href="#about">About</a>
        <a href="#team">Team orders</a>
        <a href="#faq">FAQ</a>
      </nav>

      <a class="header-btn whatsapp-link" href="#" data-message="Hi Tarlue Sports, I would like to order a custom jersey.">Order on WhatsApp</a>

      <button class="menu-toggle" id="menu-toggle" type="button" aria-label="Open menu">
        ☰
      </button>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="hero-inner">
        <div class="eyebrow">Built for the game</div>
        <h1>Wear the <span>game.</span></h1>
        <p>
          Premium custom sports jerseys for clubs, teams, and athletes. Choose your
          style and message us on WhatsApp to place your order.
        </p>
        <div class="hero-actions">
          <a class="btn" href="#shop">Shop jerseys</a>
          <a class="button-outline whatsapp-link" href="#" data-message="Hi Tarlue Sports, I need a quote for a custom jersey.">Get a quote</a>
        </div>
      </div>
    </section>

    <section class="stats">
      <div class="stat">
        <strong>24h</strong>
        <span>Quick reply</span>
      </div>
      <div class="stat">
        <strong>4.9/5</strong>
        <span>Client rating</span>
      </div>
      <div class="stat">
        <strong>2k+</strong>
        <span>Jerseys made</span>
      </div>
    </section>

    <section class="section" id="shop">
      <div class="container">
        <div class="section-head">
          <div>
            <div class="eyebrow">Popular picks</div>
            <h2>Top sellers</h2>
          </div>
          <a class="link-text whatsapp-link" href="#" data-message="Hi Tarlue Sports, please send me the full jersey catalog.">View catalog</a>
        </div>

        <div class="products">
          <article class="product-card">
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1519861531473-9200262188bf?auto=format&fit=crop&w=900&q=80" alt="Basketball jersey" />
              <span class="badge">Basketball</span>
            </div>
            <div class="product-body">
              <div class="product-meta">
                <h3>Elite Court</h3>
                <span class="price">$49</span>
              </div>
              <p>Custom basketball jersey</p>
              <a class="product-order whatsapp-link" href="#" data-message="Hi Tarlue Sports, I want to order the Elite Court jersey.">Order on WhatsApp</a>
            </div>
          </article>

          <article class="product-card">
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1574629810360-7efbbe195018?auto=format&fit=crop&w=900&q=80" alt="Soccer jersey" />
              <span class="badge">Soccer</span>
            </div>
            <div class="product-body">
              <div class="product-meta">
                <h3>Match Day</h3>
                <span class="price">$52</span>
              </div>
              <p>Custom soccer jersey</p>
              <a class="product-order whatsapp-link" href="#" data-message="Hi Tarlue Sports, I want to order the Match Day jersey.">Order on WhatsApp</a>
            </div>
          </article>

          <article class="product-card">
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1504016798967-59a258e9386d?auto=format&fit=crop&w=900&q=80" alt="Football jersey" />
              <span class="badge">Football</span>
            </div>
            <div class="product-body">
              <div class="product-meta">
                <h3>Game Day</h3>
                <span class="price">$58</span>
              </div>
              <p>Custom football jersey</p>
              <a class="product-order whatsapp-link" href="#" data-message="Hi Tarlue Sports, I want to order the Game Day jersey.">Order on WhatsApp</a>
            </div>
          </article>

          <article class="product-card">
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1538805060514-97d9cc17730c?auto=format&fit=crop&w=900&q=80" alt="Training jersey" />
              <span class="badge">Training</span>
            </div>
            <div class="product-body">
              <div class="product-meta">
                <h3>Track Kit</h3>
                <span class="price">$46</span>
              </div>
              <p>Custom training top</p>
              <a class="product-order whatsapp-link" href="#" data-message="Hi Tarlue Sports, I want to order the Track Kit.">Order on WhatsApp</a>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section class="aboutsec" id="about">
      <div class="container about-grid">
        <div class="about-copy">
          <div class="eyebrow">Why choose us</div>
          <h2>Your identity<br />on the jersey.</h2>
          <p>We create custom jerseys for teams, clubs, schools, and athletes who want premium design and standout performance. Share your colors, name, and number and we’ll take it from there.</p>

          <div class="steps">
            <article class="step">
              <div class="step-number">1</div>
              <h3>Message us</h3>
              <p>Tell us your sport, colors, and design idea.</p>
            </article>

            <article class="step">
              <div class="step-number">2</div>
              <h3>Discuss details</h3>
              <p>We’ll talk about names, numbers, sizes, and pricing.</p>
            </article>

            <article class="step">
              <div class="step-number">3</div>
              <h3>Finalize your order</h3>
              <p>Once agreed, we prepare the jersey order for you.</p>
            </article>
          </div>
        </div>

        <div class="about-image" aria-label="Sports jersey image"></div>
      </div>
    </section>

    <section class="team-banner" id="team">
      <div class="container team-grid">
        <div class="team-copy">
          <div class="eyebrow">Custom team kits</div>
          <h2>One squad.<br />One look.</h2>
          <p>Customize team uniforms for football, soccer, basketball, and more. We work with groups, clubs, and school teams to create a style that fits your identity.</p>
          <a class="btn whatsapp-link" href="#" data-message="Hi Tarlue Sports, I would like to discuss a custom team order.">Discuss a team order</a>
        </div>

        <div class="team-mark" aria-hidden="true">T</div>
      </div>
    </section>

    <section class="section" id="faq">
      <div class="container">
        <div class="section-head">
          <div>
            <div class="eyebrow">Questions</div>
            <h2>Quick answers</h2>
          </div>
        </div>

        <div class="faq-list">
          <article class="faq-item">
            <h3>How do I order?</h3>
            <p>Tap any order button and send us a message on WhatsApp with your jersey details.</p>
          </article>

          <article class="faq-item">
            <h3>Can I customize names?</h3>
            <p>Yes. We can add player names, numbers, team names, and preferred colors.</p>
          </article>

          <article class="faq-item">
            <h3>Do you offer team orders?</h3>
            <p>Yes. Contact us on WhatsApp and we’ll discuss team pricing and sizes.</p>
          </article>

          <article class="faq-item">
            <h3>Do you take online payments?</h3>
            <p>No. This website does not process online payments. Orders are arranged via WhatsApp.</p>
          </article>
        </div>
      </div>
    </section>

    <div class="contact-strip">
      <div class="container contact-inner">
        <strong>Need help with a custom order?</strong>
        <a class="wa-btn whatsapp-link" href="#" data-message="Hi Tarlue Sports, I want to ask about a custom sports jersey.">Chat on WhatsApp</a>
      </div>
    </div>
  </main>

  <footer>
    <div class="container footer-inner">
      <a href="#" class="brand" aria-label="Tarlue Sports Home">
        <svg class="brand-mark" viewBox="0 0 320 180" aria-hidden="true">
          <path fill="currentColor" d="M0 0H320L268 48L211 60V125L160 180L109 125V60L52 48L0 0ZM90 20L146 42V180H174V42L230 20H90Z" />
        </svg>
        <span>Tarlue Sports</span>
      </a>

      <div class="footer-links">
        <a href="#shop">Jerseys</a>
        <a href="#about">About</a>
        <a href="#team">Team orders</a>
        <a href="#faq">FAQ</a>
      </div>

      <div class="copyright">© <span id="year"></span> Tarlue Sports</div>
    </div>
  </footer>

  <a
    class="whatsapp-float whatsapp-link"
    href="#"
    aria-label="Chat on WhatsApp"
    data-message="Hi Tarlue Sports, I would like to ask about a custom jersey."
  >✆</a>

  <script>
    const WHATSAPP_NUMBER = "15159188539";

    document.querySelectorAll(".whatsapp-link").forEach((element) => {
      const message = element.dataset.message || "Hi Tarlue Sports, I would like to order.";
      element.href = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(message)}`;
      element.target = "_blank";
      element.rel = "noopener noreferrer";
    });

    const menuButton = document.getElementById("menu-toggle");
    const navLinks = document.getElementById("nav-links");

    menuButton.addEventListener("click", () => {
      navLinks.classList.toggle("open");
    });

    navLinks.querySelectorAll("a").forEach((link) => {
      link.addEventListener("click", () => navLinks.classList.remove("open"));
    });

    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
