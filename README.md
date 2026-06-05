<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Zenco Edible Oils Private Limited</title>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Crimson+Pro:ital,wght@0,300;0,400;0,600;1,300&family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --navy:#0d1f3c;
  --navy2:#152a4e;
  --navy3:#1a3366;
  --gold:#c9a227;
  --gold2:#e8c547;
  --gold3:#f5d87a;
  --cream:#fdf6e3;
  --cream2:#f5ead0;
  --white:#ffffff;
  --text-dark:#0a1628;
  --text-mid:#2c3e6b;
}
html{scroll-behavior:smooth}
body{font-family:'Crimson Pro',serif;background:var(--navy);color:var(--white);overflow-x:hidden}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(13,31,60,0.97);border-bottom:1px solid rgba(201,162,39,0.3);padding:0 5%}
.nav-inner{display:flex;align-items:center;justify-content:space-between;height:70px}
.nav-logo{display:flex;align-items:center;gap:12px}
.nav-logo-circle{width:44px;height:44px;border-radius:50%;border:2px solid var(--gold);background:var(--navy2);display:flex;align-items:center;justify-content:center;font-family:'Cinzel',serif;font-size:13px;font-weight:700;color:var(--gold);letter-spacing:1px}
.nav-brand{font-family:'Cinzel',serif;font-size:14px;font-weight:600;color:var(--gold2);letter-spacing:2px;line-height:1.2}
.nav-brand span{display:block;font-size:9px;font-weight:400;color:rgba(232,197,71,0.6);letter-spacing:3px}
.nav-links{display:flex;gap:32px;list-style:none}
.nav-links a{font-family:'Cinzel',serif;font-size:11px;letter-spacing:2px;color:rgba(255,255,255,0.7);text-decoration:none;transition:color 0.2s}
.nav-links a:hover{color:var(--gold2)}

/* HERO */
.hero{min-height:100vh;background:linear-gradient(160deg,#060f1f 0%,#0d1f3c 40%,#152a4e 70%,#0a1828 100%);display:flex;align-items:center;justify-content:center;text-align:center;padding:100px 5% 60px;position:relative;overflow:hidden}
.hero-rings{position:absolute;inset:0;pointer-events:none}
.ring{position:absolute;border-radius:50%;border:1px solid rgba(201,162,39,0.08)}
.ring1{width:600px;height:600px;top:50%;left:50%;transform:translate(-50%,-50%)}
.ring2{width:800px;height:800px;top:50%;left:50%;transform:translate(-50%,-50%)}
.ring3{width:1100px;height:1100px;top:50%;left:50%;transform:translate(-50%,-50%)}
.hero-content{position:relative;z-index:2;max-width:800px}
.hero-badge{display:inline-block;border:1px solid rgba(201,162,39,0.4);padding:8px 24px;font-family:'Cinzel',serif;font-size:10px;letter-spacing:4px;color:var(--gold3);margin-bottom:28px;background:rgba(201,162,39,0.05)}
.hero-title{font-family:'Cinzel',serif;font-size:clamp(32px,5vw,64px);font-weight:700;color:var(--white);line-height:1.1;margin-bottom:12px;letter-spacing:2px}
.hero-title .gold{color:var(--gold2)}
.hero-subtitle{font-family:'Cinzel',serif;font-size:clamp(11px,1.5vw,14px);letter-spacing:4px;color:rgba(201,162,39,0.7);margin-bottom:24px;font-weight:400}
.hero-divider{width:80px;height:1px;background:linear-gradient(to right,transparent,var(--gold),transparent);margin:0 auto 28px}
.hero-desc{font-size:18px;font-weight:300;color:rgba(255,255,255,0.75);line-height:1.8;max-width:560px;margin:0 auto 44px;font-style:italic}
.hero-ctas{display:flex;gap:16px;justify-content:center;flex-wrap:wrap}
.btn-gold{background:linear-gradient(135deg,var(--gold),var(--gold2));color:var(--navy);font-family:'Cinzel',serif;font-size:11px;letter-spacing:3px;padding:14px 36px;border:none;cursor:pointer;font-weight:700;text-decoration:none;display:inline-block;transition:transform 0.2s,box-shadow 0.2s}
.btn-gold:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(201,162,39,0.4)}
.btn-outline{background:transparent;color:var(--gold2);font-family:'Cinzel',serif;font-size:11px;letter-spacing:3px;padding:13px 36px;border:1px solid rgba(201,162,39,0.5);cursor:pointer;font-weight:400;text-decoration:none;display:inline-block;transition:all 0.2s}
.btn-outline:hover{background:rgba(201,162,39,0.08);border-color:var(--gold2)}

/* STRIP */
.gold-strip{background:linear-gradient(90deg,var(--gold),var(--gold2),var(--gold3),var(--gold2),var(--gold));padding:12px 0;overflow:hidden;white-space:nowrap}
.strip-inner{display:inline-flex;gap:48px;animation:scroll-strip 30s linear infinite}
.strip-item{font-family:'Cinzel',serif;font-size:10px;letter-spacing:4px;color:var(--navy);font-weight:700}
.strip-dot{color:var(--navy2);opacity:0.5}
@keyframes scroll-strip{0%{transform:translateX(0)}100%{transform:translateX(-50%)}}

/* SECTION BASE */
section{padding:100px 5%}
.section-tag{font-family:'Cinzel',serif;font-size:10px;letter-spacing:5px;color:var(--gold);margin-bottom:16px;display:block}
.section-title{font-family:'Cinzel',serif;font-size:clamp(24px,3vw,40px);font-weight:600;color:var(--white);margin-bottom:16px;letter-spacing:1px}
.section-title .gold{color:var(--gold2)}
.section-line{width:60px;height:2px;background:linear-gradient(to right,var(--gold),var(--gold2));margin-bottom:40px}
.section-desc{font-size:17px;color:rgba(255,255,255,0.65);line-height:1.9;font-weight:300;max-width:600px}

/* ABOUT */
.about{background:linear-gradient(180deg,#0d1f3c,#0a1624)}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center;max-width:1100px;margin:0 auto}
.about-visual{position:relative;display:flex;align-items:center;justify-content:center}
.about-emblem{width:280px;height:280px;border-radius:50%;border:2px solid rgba(201,162,39,0.3);background:radial-gradient(circle at center,rgba(201,162,39,0.08),rgba(13,31,60,0.9));display:flex;align-items:center;justify-content:center;position:relative}
.about-emblem::before{content:'';position:absolute;inset:-12px;border-radius:50%;border:1px solid rgba(201,162,39,0.15)}
.emblem-text{text-align:center}
.emblem-year{font-family:'Cinzel',serif;font-size:11px;letter-spacing:4px;color:var(--gold);margin-bottom:8px}
.emblem-big{font-family:'Cinzel',serif;font-size:48px;font-weight:700;color:var(--gold2);line-height:1}
.emblem-label{font-size:12px;color:rgba(255,255,255,0.5);letter-spacing:3px;font-family:'Cinzel',serif}
.about-stats{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:40px}
.stat-card{border:1px solid rgba(201,162,39,0.2);padding:20px;background:rgba(201,162,39,0.04)}
.stat-num{font-family:'Cinzel',serif;font-size:28px;font-weight:700;color:var(--gold2)}
.stat-label{font-size:13px;color:rgba(255,255,255,0.5);margin-top:4px;font-family:'Cinzel',serif;letter-spacing:1px}

/* PRODUCTS */
.products{background:linear-gradient(180deg,#0a1624,#0d1f3c)}
.products-header{text-align:center;margin-bottom:64px}
.products-header .section-line{margin:0 auto 40px}
.products-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:24px;max-width:1200px;margin:0 auto}
.product-card{border:1px solid rgba(201,162,39,0.2);background:linear-gradient(160deg,rgba(21,42,78,0.8),rgba(13,25,50,0.9));padding:36px 28px;position:relative;overflow:hidden;transition:transform 0.3s,border-color 0.3s;cursor:default}
.product-card::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(to right,transparent,var(--gold),transparent);opacity:0;transition:opacity 0.3s}
.product-card:hover{transform:translateY(-4px);border-color:rgba(201,162,39,0.5)}
.product-card:hover::before{opacity:1}
.product-icon{width:56px;height:56px;border-radius:50%;border:1px solid rgba(201,162,39,0.3);background:rgba(201,162,39,0.08);display:flex;align-items:center;justify-content:center;margin-bottom:20px;font-size:24px}
.product-name{font-family:'Cinzel',serif;font-size:16px;font-weight:600;color:var(--white);margin-bottom:8px;letter-spacing:0.5px;line-height:1.3}
.product-desc{font-size:15px;color:rgba(255,255,255,0.55);line-height:1.7;font-weight:300;margin-bottom:20px}
.product-tag{display:inline-block;font-family:'Cinzel',serif;font-size:9px;letter-spacing:2px;color:var(--gold);border:1px solid rgba(201,162,39,0.25);padding:4px 10px;background:rgba(201,162,39,0.05)}

/* PACK SIZES */
.packs{background:linear-gradient(180deg,#0d1f3c,#060f1f)}
.packs-header{text-align:center;margin-bottom:64px}
.packs-header .section-line{margin:0 auto 40px}
.packs-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:32px;max-width:1100px;margin:0 auto}
.pack-category{border:1px solid rgba(201,162,39,0.2);background:rgba(13,31,60,0.6)}
.pack-header{background:linear-gradient(135deg,rgba(201,162,39,0.15),rgba(201,162,39,0.05));padding:24px 28px;border-bottom:1px solid rgba(201,162,39,0.15)}
.pack-header-icon{font-size:28px;margin-bottom:8px}
.pack-title{font-family:'Cinzel',serif;font-size:14px;font-weight:600;color:var(--gold2);letter-spacing:1px}
.pack-subtitle{font-size:13px;color:rgba(255,255,255,0.45);margin-top:4px;font-style:italic}
.pack-body{padding:24px 28px}
.pack-sizes{list-style:none;display:flex;flex-direction:column;gap:10px}
.pack-sizes li{display:flex;align-items:center;gap:12px;font-size:15px;color:rgba(255,255,255,0.75);font-weight:300}
.pack-sizes li::before{content:'';width:6px;height:6px;border-radius:50%;background:var(--gold);flex-shrink:0}
.pack-sizes .size-value{font-family:'Cinzel',serif;font-weight:600;color:var(--white);font-size:16px}
.pack-feature{margin-top:20px;padding-top:16px;border-top:1px solid rgba(201,162,39,0.1);font-size:12px;color:rgba(201,162,39,0.6);font-family:'Cinzel',serif;letter-spacing:2px}

/* VALUES */
.values{background:linear-gradient(180deg,#060f1f,#0d1f3c)}
.values-inner{max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 2fr;gap:80px;align-items:start}
.values-grid{display:grid;grid-template-columns:1fr 1fr;gap:24px}
.value-item{padding:28px 24px;border-left:2px solid rgba(201,162,39,0.3);background:rgba(201,162,39,0.03);transition:border-color 0.2s}
.value-item:hover{border-color:var(--gold)}
.value-icon{font-size:22px;margin-bottom:12px}
.value-name{font-family:'Cinzel',serif;font-size:13px;font-weight:600;color:var(--gold2);letter-spacing:1px;margin-bottom:8px}
.value-desc{font-size:14px;color:rgba(255,255,255,0.5);line-height:1.7;font-weight:300}

/* CONTACT */
.contact{background:linear-gradient(180deg,#0d1f3c,#060f1f);text-align:center}
.contact-inner{max-width:700px;margin:0 auto}
.contact .section-line{margin:0 auto 40px}
.contact-form{margin-top:48px;display:flex;flex-direction:column;gap:16px;text-align:left}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.form-field{display:flex;flex-direction:column;gap:6px}
.form-label{font-family:'Cinzel',serif;font-size:10px;letter-spacing:3px;color:rgba(201,162,39,0.7)}
.form-input{background:rgba(21,42,78,0.5);border:1px solid rgba(201,162,39,0.2);padding:12px 16px;font-family:'Crimson Pro',serif;font-size:15px;color:var(--white);outline:none;transition:border-color 0.2s}
.form-input:focus{border-color:rgba(201,162,39,0.5)}
.form-input::placeholder{color:rgba(255,255,255,0.25)}
textarea.form-input{resize:vertical;min-height:100px}
.form-btn{align-self:center;margin-top:8px}

/* FOOTER */
footer{background:#060a14;border-top:1px solid rgba(201,162,39,0.15);padding:48px 5% 32px}
.footer-inner{max-width:1100px;margin:0 auto;display:grid;grid-template-columns:2fr 1fr 1fr;gap:60px;margin-bottom:48px}
.footer-brand-name{font-family:'Cinzel',serif;font-size:18px;font-weight:700;color:var(--gold2);letter-spacing:2px;margin-bottom:4px}
.footer-brand-sub{font-family:'Cinzel',serif;font-size:9px;letter-spacing:4px;color:rgba(201,162,39,0.4);margin-bottom:16px}
.footer-desc{font-size:14px;color:rgba(255,255,255,0.4);line-height:1.8;font-weight:300}
.footer-col-title{font-family:'Cinzel',serif;font-size:11px;letter-spacing:3px;color:var(--gold);margin-bottom:20px;padding-bottom:12px;border-bottom:1px solid rgba(201,162,39,0.15)}
.footer-links{list-style:none;display:flex;flex-direction:column;gap:10px}
.footer-links a{font-size:14px;color:rgba(255,255,255,0.45);text-decoration:none;transition:color 0.2s;font-weight:300}
.footer-links a:hover{color:var(--gold2)}
.footer-bottom{text-align:center;padding-top:24px;border-top:1px solid rgba(201,162,39,0.08);font-size:12px;color:rgba(255,255,255,0.2);font-family:'Cinzel',serif;letter-spacing:2px}

@media(max-width:768px){
  .about-grid,.packs-grid,.values-inner,.footer-inner{grid-template-columns:1fr}
  .form-row{grid-template-columns:1fr}
  .nav-links{display:none}
}
</style>
</head>
<body>

<nav>
  <div class="nav-inner">
    <div class="nav-logo">
      <div class="nav-logo-circle">Z</div>
      <div class="nav-brand">ZENCO<span>EDIBLE OILS PVT. LTD.</span></div>
    </div>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#products">Products</a></li>
      <li><a href="#packs">Packaging</a></li>
      <li><a href="#values">Quality</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</nav>

<section class="hero">
  <div class="hero-rings">
    <div class="ring ring1"></div>
    <div class="ring ring2"></div>
    <div class="ring ring3"></div>
  </div>
  <div class="hero-content">
    <div class="hero-badge">ZENCO EDIBLE OILS PRIVATE LIMITED</div>
    <h1 class="hero-title">Pure <span class="gold">Nature.</span><br>Superior <span class="gold">Quality.</span></h1>
    <div class="hero-subtitle">INDIA'S FINEST EDIBLE OILS</div>
    <div class="hero-divider"></div>
    <p class="hero-desc">Crafting premium edible oils that bring health, taste and trust to every Indian kitchen — from cold-pressed mustard to refined sunflower and beyond.</p>
    <div class="hero-ctas">
      <a href="#products" class="btn-gold">EXPLORE PRODUCTS</a>
      <a href="#contact" class="btn-outline">GET IN TOUCH</a>
    </div>
  </div>
</section>

<div class="gold-strip">
  <div class="strip-inner">
    <span class="strip-item">MUSTARD OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">SUNFLOWER OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">SOYBEAN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">RICEBRAN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">PALM OLEIN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">BPA FREE POUCHES</span><span class="strip-dot">◆</span>
    <span class="strip-item">PFA FREE PET BOTTLES</span><span class="strip-dot">◆</span>
    <span class="strip-item">TIN CANS</span><span class="strip-dot">◆</span>
    <span class="strip-item">MUSTARD OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">SUNFLOWER OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">SOYBEAN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">RICEBRAN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">PALM OLEIN OIL</span><span class="strip-dot">◆</span>
    <span class="strip-item">BPA FREE POUCHES</span><span class="strip-dot">◆</span>
    <span class="strip-item">PFA FREE PET BOTTLES</span><span class="strip-dot">◆</span>
    <span class="strip-item">TIN CANS</span><span class="strip-dot">◆</span>
  </div>
</div>

<section class="about" id="about">
  <div class="about-grid">
    <div>
      <span class="section-tag">OUR STORY</span>
      <h2 class="section-title">Rooted in <span class="gold">India's Harvest</span></h2>
      <div class="section-line"></div>
      <p class="section-desc">Zenco Edible Oils Private Limited is committed to delivering the purest, highest-quality edible oils sourced from India's finest agricultural produce. From the golden mustard fields of the Indo-Gangetic plains to sun-drenched sunflower farms, every drop carries nature's best.</p>
      <p class="section-desc" style="margin-top:20px">Our state-of-the-art refining processes preserve natural goodness while ensuring the highest standards of hygiene, safety, and taste that modern Indian families deserve.</p>
      <div class="about-stats">
        <div class="stat-card">
          <div class="stat-num">5</div>
          <div class="stat-label">Premium Varieties</div>
        </div>
        <div class="stat-card">
          <div class="stat-num">9+</div>
          <div class="stat-label">Pack Size Options</div>
        </div>
        <div class="stat-card">
          <div class="stat-num">3</div>
          <div class="stat-label">Packaging Formats</div>
        </div>
        <div class="stat-card">
          <div class="stat-num">100%</div>
          <div class="stat-label">Quality Assured</div>
        </div>
      </div>
    </div>
    <div class="about-visual">
      <div class="about-emblem">
        <div class="emblem-text">
          <div class="emblem-year">EST. IN INDIA</div>
          <div class="emblem-big">Z</div>
          <div class="emblem-label">ZENCO</div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="products" id="products">
  <div class="products-header">
    <span class="section-tag">OUR RANGE</span>
    <h2 class="section-title">Premium <span class="gold">Edible Oils</span></h2>
    <div class="section-line"></div>
    <p class="section-desc" style="margin:0 auto;text-align:center">Five exceptional varieties, each carefully selected and refined to bring out the purest flavours and health benefits.</p>
  </div>
  <div class="products-grid">
    <div class="product-card">
      <div class="product-icon">🌿</div>
      <div class="product-name">Superior Indian Mustard Oil</div>
      <p class="product-desc">Cold-pressed from the finest Indian mustard seeds, rich in omega-3 fatty acids and natural antioxidants. The quintessential oil of Indian cuisine.</p>
      <span class="product-tag">KACHI GHANI QUALITY</span>
    </div>
    <div class="product-card">
      <div class="product-icon">🌻</div>
      <div class="product-name">Refined Sunflower Oil</div>
      <p class="product-desc">Light, neutral-flavoured and high in Vitamin E. Perfect for everyday cooking, deep-frying and baking — ideal for health-conscious families.</p>
      <span class="product-tag">LIGHT & HEALTHY</span>
    </div>
    <div class="product-card">
      <div class="product-icon">🌱</div>
      <div class="product-name">Refined Soybean Oil</div>
      <p class="product-desc">Versatile and nutritious, our soybean oil is rich in polyunsaturated fats and an excellent source of Vitamin K — great for everyday use.</p>
      <span class="product-tag">HEART HEALTHY</span>
    </div>
    <div class="product-card">
      <div class="product-icon">🍚</div>
      <div class="product-name">Superior Quality Refined Ricebran Oil</div>
      <p class="product-desc">Extracted from rice bran and packed with oryzanol, this cholesterol-friendly oil has a high smoke point — perfect for Indian cooking styles.</p>
      <span class="product-tag">HIGH SMOKE POINT</span>
    </div>
    <div class="product-card">
      <div class="product-icon">🌴</div>
      <div class="product-name">Refined Palm Olein Oil</div>
      <p class="product-desc">Economical and stable for high-heat cooking. Our palm olein is refined to the highest standards for consistent quality in every pour.</p>
      <span class="product-tag">IDEAL FOR FRYING</span>
    </div>
  </div>
</section>

<section class="packs" id="packs">
  <div class="packs-header">
    <span class="section-tag">PACKAGING</span>
    <h2 class="section-title">Thoughtful <span class="gold">Pack Sizes</span></h2>
    <div class="section-line"></div>
    <p class="section-desc" style="margin:0 auto;text-align:center">Safe, sustainable packaging in formats that suit every household and commercial need — from the individual kitchen to the bulk buyer.</p>
  </div>
  <div class="packs-grid">
    <div class="pack-category">
      <div class="pack-header">
        <div class="pack-header-icon">🛍️</div>
        <div class="pack-title">Multi-Layered Pouches</div>
        <div class="pack-subtitle">BPA Free · Safe & Flexible</div>
      </div>
      <div class="pack-body">
        <ul class="pack-sizes">
          <li><span class="size-value">500 ml</span> — Half Litre Pouch</li>
          <li><span class="size-value">1 Litre</span> — Full Litre Pouch</li>
        </ul>
        <div class="pack-feature">BPA FREE · MULTI-LAYER BARRIER</div>
      </div>
    </div>
    <div class="pack-category">
      <div class="pack-header">
        <div class="pack-header-icon">🍶</div>
        <div class="pack-title">PET Bottles</div>
        <div class="pack-subtitle">PFA Free · Crystal Clear</div>
      </div>
      <div class="pack-body">
        <ul class="pack-sizes">
          <li><span class="size-value">100 ml</span> — Trial / Travel Size</li>
          <li><span class="size-value">200 ml</span> — Small Bottle</li>
          <li><span class="size-value">500 ml</span> — Half Litre</li>
          <li><span class="size-value">1 Litre</span> — Standard Bottle</li>
        </ul>
        <div class="pack-feature">PFA FREE · FOOD GRADE PET</div>
      </div>
    </div>
    <div class="pack-category">
      <div class="pack-header">
        <div class="pack-header-icon">🥫</div>
        <div class="pack-title">Tin Cans</div>
        <div class="pack-subtitle">Bulk · Commercial Grade</div>
      </div>
      <div class="pack-body">
        <ul class="pack-sizes">
          <li><span class="size-value">15 Kg</span> — Bulk Weight Tin</li>
          <li><span class="size-value">15 Litre</span> — Bulk Volume Tin</li>
        </ul>
        <div class="pack-feature">HEAVY DUTY · COMMERCIAL USE</div>
      </div>
    </div>
  </div>
</section>

<section class="values" id="values">
  <div class="values-inner">
    <div>
      <span class="section-tag">WHY ZENCO</span>
      <h2 class="section-title">Quality at Every <span class="gold">Drop</span></h2>
      <div class="section-line"></div>
      <p class="section-desc">Our commitment to quality is not just a promise — it is embedded in every process, from seed selection to the seal on your pack.</p>
    </div>
    <div class="values-grid">
      <div class="value-item">
        <div class="value-icon">🔬</div>
        <div class="value-name">Lab Tested</div>
        <p class="value-desc">Every batch undergoes rigorous quality checks for purity, acidity, and nutritional content before it leaves our facility.</p>
      </div>
      <div class="value-item">
        <div class="value-icon">🌾</div>
        <div class="value-name">Finest Sourcing</div>
        <p class="value-desc">Raw materials sourced from trusted Indian agricultural regions, ensuring freshness and natural quality in every bottle.</p>
      </div>
      <div class="value-item">
        <div class="value-icon">🛡️</div>
        <div class="value-name">Safe Packaging</div>
        <p class="value-desc">BPA-free pouches and PFA-free PET bottles ensure your family is protected from harmful chemical leaching.</p>
      </div>
      <div class="value-item">
        <div class="value-icon">🤝</div>
        <div class="value-name">Trusted Partner</div>
        <p class="value-desc">From retail households to bulk commercial buyers, we deliver consistency, reliability, and the Zenco promise.</p>
      </div>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="contact-inner">
    <span class="section-tag">REACH US</span>
    <h2 class="section-title">Get in <span class="gold">Touch</span></h2>
    <div class="section-line"></div>
    <p class="section-desc" style="margin:0 auto">Whether you're a retailer, distributor or a household customer, we'd love to hear from you. Drop us a message and we'll get back to you promptly.</p>
    <div class="contact-form">
      <div class="form-row">
        <div class="form-field">
          <label class="form-label">YOUR NAME</label>
          <input type="text" class="form-input" placeholder="Full name">
        </div>
        <div class="form-field">
          <label class="form-label">MOBILE / EMAIL</label>
          <input type="text" class="form-input" placeholder="Contact details">
        </div>
      </div>
      <div class="form-row">
        <div class="form-field">
          <label class="form-label">PRODUCT INTEREST</label>
          <input type="text" class="form-input" placeholder="e.g. Mustard Oil, Sunflower Oil">
        </div>
        <div class="form-field">
          <label class="form-label">ENQUIRY TYPE</label>
          <input type="text" class="form-input" placeholder="Retail / Wholesale / Distributor">
        </div>
      </div>
      <div class="form-field">
        <label class="form-label">YOUR MESSAGE</label>
        <textarea class="form-input" placeholder="Tell us about your requirements..."></textarea>
      </div>
      <div class="form-btn">
        <a href="#" class="btn-gold">SEND ENQUIRY</a>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="footer-inner">
    <div>
      <div class="footer-brand-name">ZENCO</div>
      <div class="footer-brand-sub">EDIBLE OILS PRIVATE LIMITED</div>
      <p class="footer-desc">Bringing nature's finest oils to Indian kitchens — pure, safe, and crafted with care. From our fields to your family table.</p>
    </div>
    <div>
      <div class="footer-col-title">PRODUCTS</div>
      <ul class="footer-links">
        <li><a href="#products">Mustard Oil</a></li>
        <li><a href="#products">Sunflower Oil</a></li>
        <li><a href="#products">Soybean Oil</a></li>
        <li><a href="#products">Ricebran Oil</a></li>
        <li><a href="#products">Palm Olein Oil</a></li>
      </ul>
    </div>
    <div>
      <div class="footer-col-title">QUICK LINKS</div>
      <ul class="footer-links">
        <li><a href="#about">About Us</a></li>
        <li><a href="#packs">Packaging</a></li>
        <li><a href="#values">Quality</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">© 2025 ZENCO EDIBLE OILS PRIVATE LIMITED · ALL RIGHTS RESERVED</div>
</footer>

</body>
</html>
