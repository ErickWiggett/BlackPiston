<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Black Piston — Motorcycle Spares</title>
  <style>
    :root{
      --bg:#0b0b0b; --card:#111214; --muted:#9aa0a6; --accent:#d32f2f; --steel:#bfc7ca;
      --maxw:1100px;
      font-family:Inter, sans-serif;
    }
    body{margin:0; background:var(--bg); color:#e6e6e6;}
    .wrap{max-width:var(--maxw); margin:0 auto; padding:32px}
    header{display:flex;justify-content:space-between;align-items:center;padding:18px 0}
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:60px;height:60px;background:#111;border-radius:10px;display:flex;align-items:center;justify-content:center}
    nav a{color:var(--muted);margin-left:18px;text-decoration:none;font-weight:600}
    nav a:hover{color:var(--steel)}
    .hero{display:grid;grid-template-columns:1fr 400px;gap:28px;align-items:center;padding:36px 0}
    .hero-left h1{font-size:44px;margin:0 0 12px}
    .hero-left p{color:var(--muted);line-height:1.6}
    .cta{margin-top:20px;display:flex;gap:12px}
    .btn{padding:12px 18px;border-radius:8px;font-weight:700;border:0;cursor:pointer}
    .btn-primary{background:var(--accent);color:white}
    .btn-ghost{background:transparent;border:1px solid #222;color:var(--steel)}
    .section{padding:56px 0;border-top:1px solid rgba(255,255,255,0.03)}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px}
    .card{background:var(--card);padding:14px;border-radius:10px;box-shadow:0 6px 18px rgba(0,0,0,0.6);border:1px solid rgba(255,255,255,0.02)}
    .card img{width:100%;height:130px;object-fit:cover;border-radius:8px}
    .muted{color:var(--muted);font-size:14px}
    footer{padding:28px 0;color:var(--muted);border-top:1px solid rgba(255,255,255,0.03);display:flex;justify-content:space-between;align-items:center}
    @media (max-width:940px){.hero{grid-template-columns:1fr}.hero-left h1{font-size:32px}}
  </style>
</head>
<body>
<div class="wrap">
  <header>
    <div class="brand">
      <div class="logo">
        <img src="assets/logo.svg" alt="Black Piston Logo" width="36"/>
      </div>
      <div>
        <div style="font-weight:800;letter-spacing:1px">BLACK PISTON</div>
        <div class="muted">Quality new motorcycle spares</div>
      </div>
    </div>
    <nav>
      <a href="#parts">Parts</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-left">
      <h1>Black Piston — fresh spares for every ride</h1>
      <p>High-quality new motorcycle parts, fast sourcing, and reliable fitting. We stock common parts for most popular makes and can source what you need.</p>
      <div class="cta">
        <a class="btn btn-primary" href="#parts">View parts</a>
        <a class="btn btn-ghost" href="#contact">Contact us</a>
      </div>
    </div>
    <div>
      <img src="assets/hero.jpg" alt="Motorcycle" style="width:100%;border-radius:12px"/>
    </div>
  </section>

  <section id="parts" class="section">
    <h2>Parts Catalogue</h2>
    <p class="muted">Browse our range of new motorcycle parts. Add new items easily by duplicating a card.</p>
    <div class="grid" id="partsGrid">
      <article class="card">
        <img src="assets/parts/chain.jpg" alt="Drive Chain"/>
        <div style="margin-top:10px;font-weight:800">Drive Chain — Standard</div>
        <div class="muted">Suitable for most commuter bikes. Size options available.</div>
      </article>
      <article class="card">
        <img src="assets/parts/brakepads.jpg" alt="Brake Pads"/>
        <div style="margin-top:10px;font-weight:800">Brake Pads — Front/Rear</div>
        <div class="muted">High-friction compound for reliable stopping.</div>
      </article>
      <article class="card">
        <img src="assets/parts/airfilter.jpg" alt="Air Filter"/>
        <div style="margin-top:10px;font-weight:800">Air Filter — OEM Fit</div>
        <div class="muted">Paper & reusable foam options available.</div>
      </article>
      <article class="card">
        <img src="assets/parts/sparkplug.jpg" alt="Spark Plug"/>
        <div style="margin-top:10px;font-weight:800">Spark Plugs</div>
        <div class="muted">Premium iridium & standard options.</div>
      </article>
      <article class="card">
        <img src="assets/parts/oilfilter.jpg" alt="Oil Filter"/>
        <div style="margin-top:10px;font-weight:800">Oil Filter</div>
        <div class="muted">OEM-equivalent spin-on and cartridge filters.</div>
      </article>
      <article class="card">
        <img src="assets/parts/lever.jpg" alt="Lever"/>
        <div style="margin-top:10px;font-weight:800">Clutch / Brake Levers</div>
        <div class="muted">Adjustable replacements — OEM fitment options.</div>
      </article>
    </div>
  </section>

  <section id="contact" class="section">
    <h2>Contact</h2>
    <p class="muted">Send us your bike make, model, and the part you need. We'll check availability and get back to you.</p>
    <form onsubmit="event.preventDefault(); alert('Message sent (demo).');" style="margin-top:12px">
      <input placeholder="Your name" required /><br><br>
      <input placeholder="Phone or email" required /><br><br>
      <textarea rows="4" placeholder="e.g. 2018 Honda CB300R — front brake pads" required></textarea><br><br>
      <button class="btn btn-primary" type="submit">Send Enquiry</button>
    </form>
  </section>

  <footer>
    <div>© <strong>Black Piston</strong> — All rights reserved</div>
    <div class="muted">Showcase site</div>
  </footer>
</div>
</body>
</html>
