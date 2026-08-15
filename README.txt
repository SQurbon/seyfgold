<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="SEYFGOLD — uy, ofis va biznes uchun premium seyflar. Turli o'lcham va himoya darajalaridagi seyflar, yetkazib berish va maslahat.">
  <title>SEYFGOLD — Premium Seyflar</title>
  <style>
    :root{
      --bg:#080808; --card:#111111; --gold:#d4af37; --gold2:#f3d477;
      --text:#f7f4ec; --muted:#a9a59b; --line:#2a2926; --white:#fff;
      --max:1180px; --radius:22px;
    }
    *{box-sizing:border-box;margin:0;padding:0}
    html{scroll-behavior:smooth}
    body{font-family:Inter,Arial,sans-serif;background:var(--bg);color:var(--text);line-height:1.55}
    a{text-decoration:none;color:inherit}
    img{max-width:100%;display:block}
    .container{width:min(calc(100% - 32px),var(--max));margin:auto}
    .top{background:#0d0d0d;border-bottom:1px solid var(--line);font-size:13px;color:var(--muted)}
    .top .container{display:flex;justify-content:space-between;gap:15px;padding:9px 0}
    header{position:sticky;top:0;z-index:50;background:rgba(8,8,8,.9);backdrop-filter:blur(14px);border-bottom:1px solid rgba(212,175,55,.14)}
    nav{min-height:72px;display:flex;align-items:center;justify-content:space-between;gap:20px}
    .brand{font-size:25px;font-weight:900;letter-spacing:3px;color:var(--gold2)}
    .brand span{display:block;font-size:9px;letter-spacing:2px;color:var(--muted);font-weight:600;margin-top:-3px}
    .links{display:flex;gap:24px;align-items:center;color:#d8d5cd;font-size:14px}
    .links a:hover{color:var(--gold2)}
    .btn{display:inline-flex;align-items:center;justify-content:center;gap:9px;padding:13px 19px;border-radius:999px;font-weight:800;border:1px solid #8f7627;background:linear-gradient(135deg,#f0d16b,#b78c1d);color:#0a0a0a;box-shadow:0 8px 28px rgba(212,175,55,.14);transition:.2s}
    .btn:hover{transform:translateY(-2px);filter:brightness(1.05)}
    .btn.dark{background:#111;color:#f4e4ae;border-color:#3b3526;box-shadow:none}
    .hero{padding:28px 0 0}
    .hero-card{position:relative;overflow:hidden;border:1px solid #3a3322;border-radius:28px;min-height:520px;background:#0b0b0b}
    .hero-card img{width:100%;height:100%;min-height:520px;object-fit:cover;opacity:.92}
    .hero-overlay{position:absolute;inset:0;background:linear-gradient(90deg,rgba(0,0,0,.72),rgba(0,0,0,.18) 58%,rgba(0,0,0,.22))}
    .hero-content{position:absolute;inset:0;display:flex;align-items:center;padding:55px;max-width:680px}
    .eyebrow{color:var(--gold2);font-size:12px;font-weight:800;letter-spacing:3px;text-transform:uppercase;margin-bottom:15px}
    h1{font-size:clamp(42px,6vw,76px);line-height:.98;letter-spacing:-2px;margin-bottom:20px}
    .hero p{font-size:18px;color:#ddd8cc;max-width:570px}
    .hero-actions{display:flex;flex-wrap:wrap;gap:12px;margin-top:28px}
    section{padding:78px 0}
    .section-head{display:flex;align-items:end;justify-content:space-between;gap:25px;margin-bottom:30px}
    .kicker{color:var(--gold2);font-size:12px;letter-spacing:2px;font-weight:800;text-transform:uppercase}
    h2{font-size:clamp(30px,4vw,48px);line-height:1.05;margin-top:8px}
    .sub{color:var(--muted);max-width:650px}
    .features{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
    .feature,.card,.contact-box,.faq details{background:linear-gradient(180deg,#141414,#0d0d0d);border:1px solid var(--line);border-radius:var(--radius)}
    .feature{padding:25px}
    .icon{font-size:26px;margin-bottom:14px}
    .feature h3{font-size:16px;margin-bottom:6px}
    .feature p{color:var(--muted);font-size:14px}
    .products{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{overflow:hidden}
    .product-img{height:245px;background:linear-gradient(135deg,#1a1a1a,#080808);display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden}
    .product-img img{width:100%;height:100%;object-fit:contain;padding:10px;filter:drop-shadow(0 18px 24px rgba(0,0,0,.35));transition:.25s}
    .card:hover .product-img img{transform:scale(1.025)}
    .badge{position:absolute;top:14px;left:14px;background:#e5c65f;color:#17120a;padding:6px 10px;border-radius:999px;font-size:11px;font-weight:900}
    .card-body{padding:21px}
    .card-body h3{font-size:20px;margin-bottom:7px}
    .card-body p{color:var(--muted);font-size:14px;min-height:44px}
    .specs{display:flex;gap:8px;flex-wrap:wrap;margin:14px 0}
    .spec{border:1px solid #302d27;color:#bdb8ac;padding:5px 9px;border-radius:999px;font-size:11px}
    .card-foot{display:flex;align-items:center;justify-content:space-between;gap:10px}
    .price{font-size:19px;font-weight:900;color:var(--gold2)}
    .about{display:grid;grid-template-columns:1fr 1fr;gap:25px;align-items:stretch}
    .about-box{padding:34px;background:linear-gradient(145deg,#15130f,#0d0d0d);border:1px solid #3a3322;border-radius:var(--radius)}
    .about-box p{color:#c6c1b5;margin-top:14px}
    .checks{display:grid;gap:12px;margin-top:22px}
    .check{display:flex;gap:10px;align-items:flex-start;color:#ddd8cd}
    .check b{color:var(--gold2)}
    .contact{background:radial-gradient(circle at 75% 30%,rgba(212,175,55,.12),transparent 32%),#0e0e0e;border-top:1px solid #2e291e;border-bottom:1px solid #2e291e}
    .contact-grid{display:grid;grid-template-columns:1.1fr .9fr;gap:25px}
    .contact-box{padding:30px}
    .contact-list{display:grid;gap:13px;margin-top:22px}
    .contact-item{display:flex;gap:13px;align-items:center;padding:14px;border:1px solid #292722;border-radius:15px;background:#0b0b0b}
    .contact-item strong{display:block}
    .contact-item small{color:var(--muted)}
    .faq{display:grid;gap:10px}
    .faq details{padding:18px 20px}
    .faq summary{cursor:pointer;font-weight:800}
    .faq p{color:var(--muted);padding-top:12px}
    footer{padding:30px 0 45px;border-top:1px solid var(--line);color:var(--muted);font-size:13px}
    footer .container{display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap}
    .float{position:fixed;right:20px;bottom:20px;z-index:60}
    .float a{width:56px;height:56px;border-radius:50%;display:grid;place-items:center;background:#1687e8;color:white;font-size:23px;box-shadow:0 10px 30px rgba(0,0,0,.45);border:2px solid rgba(255,255,255,.12)}
    @media(max-width:900px){
      .links{display:none}.features{grid-template-columns:repeat(2,1fr)}
      .products{grid-template-columns:1fr 1fr}.about,.contact-grid{grid-template-columns:1fr}
      .hero-content{padding:32px}.hero-card,.hero-card img{min-height:580px}
    }
    @media(max-width:600px){
      .top{display:none}.container{width:min(calc(100% - 22px),var(--max))}
      nav{min-height:64px}.brand{font-size:21px}
      .features,.products{grid-template-columns:1fr}
      section{padding:55px 0}.hero{padding-top:12px}
      .hero-card{border-radius:20px}.hero-content{padding:25px;align-items:end;padding-bottom:38px}
      .hero-card img{min-height:620px;object-position:center}
      h1{font-size:46px}.hero p{font-size:16px}.hero-actions .btn{width:100%}
      .section-head{display:block}.section-head .sub{margin-top:14px}
    }
  </style>
</head>
<body>
  <div class="top"><div class="container"><span>SEYFGOLD • Premium seyflar</span><span>Toshkent • O‘zbekiston bo‘ylab yetkazib berish</span></div></div>

  <header>
    <nav class="container">
      <a class="brand" href="#top">SEYFGOLD<span>SECURITY • PREMIUM QUALITY</span></a>
      <div class="links">
        <a href="#products">Seyflar</a><a href="#about">Biz haqimizda</a><a href="#delivery">Yetkazib berish</a><a href="#faq">FAQ</a>
      </div>
      <a class="btn" href="#contact">Bog‘lanish</a>
    </nav>
  </header>

  <main id="top">
    <div class="container hero">
      <div class="hero-card">
        <img src="hero-banner.png" alt="SEYFGOLD premium seyflar">
        <div class="hero-overlay"></div>
        <div class="hero-content">
          <div>
            <div class="eyebrow">Premium security solutions</div>
            <h1>Qimmatli narsalaringiz uchun ishonchli himoya.</h1>
            <p>Uy, ofis va biznes uchun turli hajm va himoya darajasidagi zamonaviy seyflar. Tanlashda yordam beramiz.</p>
            <div class="hero-actions">
              <a class="btn" href="#products">Seyflarni ko‘rish</a>
              <a class="btn dark" href="#contact">Maslahat olish</a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <section>
      <div class="container">
        <div class="section-head">
          <div><div class="kicker">Nega SEYFGOLD?</div><h2>Premium xizmat. Oddiy xarid.</h2></div>
          <p class="sub">Mijozga kerak bo‘lgan ma’lumot bir joyda: mahsulot, maslahat, yetkazib berish va tezkor aloqa.</p>
        </div>
        <div class="features">
          <div class="feature"><div class="icon">🛡️</div><h3>Ishonchli himoya</h3><p>Uy va biznesdagi muhim buyumlarni saqlash uchun mos yechimlar.</p></div>
          <div class="feature"><div class="icon">🔐</div><h3>Turli qulflash tizimlari</h3><p>Mexanik, kalitli va elektron variantlardan tanlash imkoniyati.</p></div>
          <div class="feature"><div class="icon">🚚</div><h3>Yetkazib berish</h3><p>Kelishilgan manzilga yetkazib berish imkoniyati.</p></div>
          <div class="feature"><div class="icon">💎</div><h3>Premium ko‘rinish</h3><p>Interyerga mos, zamonaviy va sifatli dizayndagi modellar.</p></div>
        </div>
      </div>
    </section>

    <section id="products">
      <div class="container">
        <div class="section-head">
          <div><div class="kicker">Mahsulotlar</div><h2>Seyfni ehtiyojingizga qarab tanlang</h2></div>
          <p class="sub">SEYFGOLD premium kolleksiyasidan tanlangan modellar. O‘lcham va narxlar mahsulot kartasida ko‘rsatilgan.</p>
        </div>
        <div class="products">
          <article class="card"><div class="product-img"><img src="home-safe-premium.png" alt="Home Safe Premium AS100"><span class="badge">UY UCHUN</span></div><div class="card-body"><h3>Home Safe Premium</h3><p>Model AS100 — uy uchun premium, zamonaviy va ishonchli seyf.</p><div class="specs"><span class="spec">Model: AS100</span><span class="spec">100 × 52 × 44 sm</span><span class="spec">Premium</span></div><div class="card-foot"><span class="price">19 300 000 so‘m</span><a class="btn" href="#contact">So‘rash</a></div></div></article>
          <article class="card"><div class="product-img"><img src="assets/office-secure.png" alt="Office Secure XZ80"><span class="badge">OFIS</span></div><div class="card-body"><h3>Office Secure</h3><p>Model XZ80 — hujjatlar, pul va muhim buyumlarni saqlash uchun amaliy yechim.</p><div class="specs"><span class="spec">Model: XZ80</span><span class="spec">80 × 48 × 40 sm</span><span class="spec">Ofis</span></div><div class="card-foot"><span class="price">5 900 000 so‘m</span><a class="btn" href="#contact">So‘rash</a></div></div></article>
          <article class="card"><div class="product-img"><img src="assets/business-pro.png" alt="Business Pro HM60"><span class="badge">BIZNES</span></div><div class="card-body"><h3>Business Pro</h3><p>Model HM60 — biznes uchun professional foydalanishga mos premium seyf.</p><div class="specs"><span class="spec">Model: HM60</span><span class="spec">60 × 41 × 37 sm</span><span class="spec">Professional</span></div><div class="card-foot"><span class="price">10 900 000 so‘m</span><a class="btn" href="#contact">So‘rash</a></div></div></article>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="container about">
        <div class="about-box">
          <div class="kicker">SEYFGOLD</div><h2>Sizga mos seyfni topishga yordam beramiz.</h2>
          <p>Seyf tanlashda o‘lcham, o‘rnatish joyi, saqlanadigan buyumlar va kerakli himoya darajasi muhim. Biz sizning vaziyatingizga mos variantni tavsiya qilamiz.</p>
          <div class="checks">
            <div class="check">✓ <span><b>Maslahat:</b> ehtiyojingizga mos modelni tanlash</span></div>
            <div class="check">✓ <span><b>Tanlov:</b> turli hajm va dizaynlar</span></div>
            <div class="check">✓ <span><b>Qulaylik:</b> buyurtma va aloqa bir necha bosqichda</span></div>
          </div>
        </div>
        <div class="about-box" id="delivery">
          <div class="kicker">Xizmat</div><h2>Yetkazib berish va buyurtma</h2>
          <p>Modelni tanlang yoki bizga yozing. Manzilingizni yuboring — mavjudlik, narx va yetkazib berish shartlarini aniqlashtiramiz.</p>
          <div class="hero-actions"><a class="btn" href="#contact">Buyurtma berish</a><a class="btn dark" href="#faq">Savollar</a></div>
        </div>
      </div>
    </section>

    <section id="faq">
      <div class="container">
        <div class="section-head"><div><div class="kicker">FAQ</div><h2>Ko‘p so‘raladigan savollar</h2></div></div>
        <div class="faq">
          <details><summary>Qaysi seyf menga mos?</summary><p>Saqlanadigan buyumlar, kerakli hajm, o‘rnatish joyi va qulflash turiga qarab tanlanadi. Bizga yozsangiz, mos variantlarni tavsiya qilamiz.</p></details>
          <details><summary>Narxlar qanday?</summary><p>Narx model, o‘lcham va funksiyaga qarab o‘zgaradi. Aniq narx uchun kerakli modelni yuboring yoki biz bilan bog‘laning.</p></details>
          <details><summary>Yetkazib berish bormi?</summary><p>Ha, yetkazib berish shartlari manzilga qarab kelishiladi.</p></details>
          <details><summary>Elektron qulf paroli unutilsa nima bo‘ladi?</summary><p>Modelga qarab tiklash usuli farq qiladi. Model nomi yoki fotosini yuborsangiz, yechim bo‘yicha yordam beramiz.</p></details>
        </div>
      </div>
    </section>

    <section class="contact" id="contact">
      <div class="container contact-grid">
        <div>
          <div class="kicker">Bog‘lanish</div><h2>Seyf tanlash bo‘yicha maslahat oling.</h2>
          <p class="sub" style="margin-top:14px">Telegram orqali yozing yoki email yuboring. Biz bilan qulay usulda bog‘laning — tezkor maslahat va buyurtmalar uchun.</p>
          <div class="contact-list">
            <!-- O'Z KONTAKTLARINGIZNI SHU YERDA ALMASHTIRING -->
            <a class="contact-item" href="https://t.me/maksudovb" target="_blank"><span>✈️</span><span><strong>Telegram</strong><small>@maksudovb</small></span></a>
            <a class="contact-item" href="mailto:abdullaw410oc@gmail.com"><span>✉️</span><span><strong>Email</strong><small>abdullaw410oc@gmail.com</small></span></a>
            <a class="contact-item" href="tel:+998330867271"><span>📞</span><span><strong>Telefon</strong><small>+998 33 086 72 71</small></span></a>
          </div>
        </div>
        <div class="contact-box">
          <div class="kicker">Tezkor buyurtma</div>
          <h3 style="font-size:28px;margin:8px 0 18px">“Menga seyf kerak” deb yozing</h3>
          <p style="color:var(--muted)">Telegram tugmasi orqali mijozni to‘g‘ridan-to‘g‘ri sizga olib borish mumkin. Keyinchalik bu yerga WhatsApp, Instagram yoki buyurtma formasini ham qo‘shish mumkin.</p>
          <div class="hero-actions"><a class="btn" href="https://t.me/maksudovb" target="_blank">Telegramga yozish</a></div>
        </div>
      </div>
    </section>
  </main>

  <footer><div class="container"><span>© 2026 SEYFGOLD. Barcha huquqlar himoyalangan.</span><span>Premium seyflar • Toshkent • O‘zbekiston</span></div></footer>
  <div class="float"><a href="https://t.me/maksudovb" target="_blank" aria-label="Telegram">✈️</a></div>
</body>
</html>
