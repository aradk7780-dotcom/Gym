<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>باشگاه بدنسازی | Fitness Club</title>
  <meta name="description" content="سایت حرفه‌ای باشگاه بدنسازی: معرفی، برنامه‌ها، مربیان، قیمت‌ها، گالری، وبلاگ، و فرم عضویت آنلاین." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b0b0f;          /* پس‌زمینه تیره لوکس */
      --card:#13131a;        /* کارت‌ها */
      --soft:#1b1b25;        /* سطوح نرم */
      --text:#eaeaf2;        /* متن اصلی */
      --muted:#b6b6c6;       /* متن فرعی */
      --primary:#f43f5e;     /* قرمز شارپی */
      --accent:#22d3ee;      /* آبی فیروزه‌ای */
      --ok:#10b981;          /* سبز تایید */
      --warn:#f59e0b;        /* هشدار */
      --error:#ef4444;
      --radius:18px;
      --shadow:0 10px 30px rgba(0,0,0,.35);
      --shadow-soft:0 6px 18px rgba(0,0,0,.25);
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:linear-gradient(180deg,#0a0a0d, #0f0f16);color:var(--text);font-family:'Vazirmatn',system-ui,Segoe UI,Roboto,Arial,sans-serif}
    a{color:inherit;text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1200px,92%);margin-inline:auto}

    /* Header */
    header{position:sticky;top:0;z-index:999;background:rgba(13,13,20,.7);backdrop-filter:saturate(140%) blur(10px);border-bottom:1px solid rgba(255,255,255,.05)}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 0}
    .brand{display:flex;align-items:center;gap:10px}
    .logo{width:38px;height:38px;border-radius:12px;background:linear-gradient(135deg,var(--primary),#7c3aed);display:grid;place-items:center;color:white;font-weight:800;box-shadow:var(--shadow-soft)}
    .brand h1{font-size:17px;margin:0;letter-spacing:.2px}
    nav ul{display:flex;gap:20px;list-style:none;margin:0;padding:0}
    nav a{padding:8px 12px;border-radius:12px;transition:.2s}
    nav a:hover{background:rgba(255,255,255,.06)}
    .cta{background:linear-gradient(135deg,var(--primary),#fb7185);padding:10px 16px;border-radius:14px;font-weight:700;box-shadow:var(--shadow)}

    /* Hero */
    .hero{position:relative;isolation:isolate}
    .hero .bg{
      position:absolute;inset:0;z-index:-1;opacity:.22;pointer-events:none;
      background: radial-gradient(900px 600px at 80% -10%, rgba(244,63,94,.7), transparent 60%),
                  radial-gradient(700px 500px at 10% 0%, rgba(34,211,238,.6), transparent 55%),
                  url('https://images.unsplash.com/photo-1517836357463-d25dfeac3438?q=80&w=2060&auto=format&fit=crop');
      background-size:cover; background-position:center; filter:grayscale(40%) contrast(110%);
    }
    .hero .container{display:grid;grid-template-columns:1.2fr .8fr;gap:30px;align-items:center;min-height:72vh;padding:34px 0}
    .kpis{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:22px}
    .kpi{background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.08);padding:16px;border-radius:16px;text-align:center}
    .kpi h3{margin:0;font-size:22px}
    .kpi p{margin:6px 0 0;color:var(--muted);font-size:13px}
    .hero-card{background:rgba(19,19,26,.8);border:1px solid rgba(255,255,255,.08);padding:18px;border-radius:18px;box-shadow:var(--shadow-soft)}
    .hero h2{font-size:42px;line-height:1.2;margin:0 0 12px}
    .hero h2 .accent{background:linear-gradient(135deg,var(--accent),#60a5fa);-webkit-background-clip:text;background-clip:text;color:transparent}
    .hero p{color:var(--muted);margin:0 0 20px}
    .hero .actions{display:flex;gap:12px;flex-wrap:wrap}
    .btn{border:1px solid rgba(255,255,255,.12);padding:12px 16px;border-radius:14px;background:#151520;cursor:pointer;color:var(--text);font-weight:600;transition:.2s}
    .btn:hover{transform:translateY(-1px);box-shadow:var(--shadow-soft)}
    .btn.primary{background:linear-gradient(135deg,var(--primary),#fb7185);border:none}

    /* Sections */
    section{padding:64px 0;border-top:1px solid rgba(255,255,255,.06)}
    section .head{display:flex;align-items:flex-end;justify-content:space-between;gap:16px;margin-bottom:28px}
    .title{font-size:28px;margin:0}
    .subtitle{margin:6px 0 0;color:var(--muted)}

    /* Cards grid */
    .grid{display:grid;grid-template-columns:repeat(12,1fr);gap:18px}
    .col-4{grid-column:span 4}
    .col-6{grid-column:span 6}
    .col-8{grid-column:span 8}
    .card{background:var(--card);border:1px solid rgba(255,255,255,.08);border-radius:18px;overflow:hidden;box-shadow:var(--shadow-soft)}
    .card-body{padding:18px}
    .chip{display:inline-flex;align-items:center;gap:8px;font-size:12px;color:#fff;background:linear-gradient(135deg,#4f46e5,#22d3ee);border-radius:999px;padding:6px 10px}

    /* About */
    .about p{color:var(--muted)}

    /* Programs */
    .program{display:flex;gap:14px;align-items:flex-start}
    .program .icon{width:44px;height:44px;border-radius:12px;display:grid;place-items:center;background:linear-gradient(135deg,#1f2937,#111827);border:1px solid rgba(255,255,255,.08)}
    .program h4{margin:4px 0 6px}
    .program p{margin:0;color:var(--muted)}

    /* Pricing */
    .pricing{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .price-card{position:relative}
    .price{font-size:34px;font-weight:800}
    .badge{position:absolute;top:14px;left:14px}
    .features{margin:14px 0 0;padding:0;list-style:none}
    .features li{display:flex;align-items:center;gap:8px;margin:10px 0;color:var(--muted)}

    /* Trainers */
    .trainer{display:flex;gap:14px;align-items:center}
    .trainer img{width:72px;height:72px;border-radius:16px;object-fit:cover;border:2px solid rgba(255,255,255,.08)}

    /* Gallery */
    .gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
    .gallery a{border-radius:14px;overflow:hidden;border:1px solid rgba(255,255,255,.08)}
    .lightbox{position:fixed;inset:0;display:none;place-items:center;background:rgba(0,0,0,.85);z-index:9999}
    .lightbox img{max-width:92%;max-height:88%;border-radius:16px}

    /* Blog */
    .blog .meta{display:flex;gap:12px;color:var(--muted);font-size:12px}

    /* Contact & Form */
    .contact-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:18px}
    form{display:grid;gap:12px}
    input, select, textarea{background:#101018;border:1px solid rgba(255,255,255,.08);padding:12px 14px;border-radius:12px;color:var(--text);outline:none}
    input:focus, select:focus, textarea:focus{border-color:var(--accent);box-shadow:0 0 0 3px rgba(34,211,238,.15)}
    .form-row{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
    .note{font-size:12px;color:var(--muted)}
    .map{height:100%;min-height:320px;border-radius:16px;overflow:hidden;border:1px solid rgba(255,255,255,.08)}

    /* Footer */
    footer{padding:28px 0;border-top:1px solid rgba(255,255,255,.06);color:var(--muted)}

    /* Responsive */
    @media (max-width: 1000px){
      .hero .container{grid-template-columns:1fr}
      .kpis{grid-template-columns:repeat(3,1fr)}
      .pricing{grid-template-columns:1fr 1fr}
      .contact-grid{grid-template-columns:1fr}
    }
    @media (max-width: 720px){
      nav ul{display:none}
      .kpis{grid-template-columns:1fr 1fr}
      .gallery{grid-template-columns:1fr 1fr}
      .pricing{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr}
      .col-4,.col-6,.col-8{grid-column:span 1}
      .form-row{grid-template-columns:1fr}
      .hero h2{font-size:34px}
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo">🏋️‍♂️</div>
        <h1>باشگاه <strong>FitnessPro</strong></h1>
      </div>
      <nav>
        <ul>
          <li><a href="#home">خانه</a></li>
          <li><a href="#about">درباره ما</a></li>
          <li><a href="#programs">برنامه‌ها</a></li>
          <li><a href="#trainers">مربیان</a></li>
          <li><a href="#pricing">قیمت‌ها</a></li>
          <li><a href="#gallery">گالری</a></li>
          <li><a href="#blog">وبلاگ</a></li>
          <li><a href="#contact">تماس</a></li>
        </ul>
      </nav>
      <a class="cta" href="#signup">ثبت‌نام آنلاین</a>
    </div>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <div class="bg" aria-hidden="true"></div>
    <div class="container">
      <div>
        <div class="chip">شروع قدرتمند امروز شما</div>
        <h2>بدن رویایی‌ات رو <span class="accent">بساز</span> — با برنامه‌های حرفه‌ای و مربیان مجرب</h2>
        <p>تجربه تمرین در فضایی حرفه‌ای با تجهیزات کامل، کلاس‌های گروهی هیجان‌انگیز و برنامه‌های شخصی‌سازی‌شده برای هر سطح.</p>
        <div class="actions">
          <a class="btn primary" href="#signup">همین الان عضو شو</a>
          <a class="btn" href="#programs">دیدن برنامه‌ها</a>
        </div>
        <div class="kpis">
          <div class="kpi"><h3>+1200</h3><p>اعضای فعال</p></div>
          <div class="kpi"><h3>+25</h3><p>کلاس هفتگی</p></div>
          <div class="kpi"><h3>+10</h3><p>مربی متخصص</p></div>
        </div>
      </div>
      <div class="hero-card">
        <h3 style="margin-top:0">عضویت آزمایشی ۳روزه</h3>
        <p class="subtitle">با دسترسی کامل به تجهیزات و یک جلسه مشاوره رایگان</p>
        <form id="trialForm">
          <div class="form-row">
            <input name="name" placeholder="نام و نام خانوادگی" required>
            <input name="phone" placeholder="شماره تماس" inputmode="tel" required>
          </div>
          <select name="goal">
            <option value="عضله سازی">هدف: عضله‌سازی</option>
            <option value="کاهش وزن">هدف: کاهش وزن</option>
            <option value="تناسب اندام">هدف: تناسب اندام</option>
          </select>
          <button class="btn primary" type="submit">درخواست عضویت آزمایشی</button>
          <div id="trialMsg" class="note"></div>
        </form>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="about">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">درباره باشگاه</h3>
          <p class="subtitle">بیش از ۵ سال کنار شما برای رسیدن به بهترین نسخه‌ی خودتان</p>
        </div>
        <span class="chip">تجهیزات بروز • محیط حرفه‌ای</span>
      </div>
      <div class="grid">
        <div class="card col-8">
          <img src="https://images.unsplash.com/photo-1517821362838-8ddbfbf4ff0b?q=80&w=2070&auto=format&fit=crop" alt="محیط باشگاه">
        </div>
        <div class="card col-4">
          <div class="card-body">
            <h4>ماموریت ما</h4>
            <p>ارائه‌ی تجربه‌ی تمرینی ایمن، علمی و انگیزشی برای تمامی سنین و سطوح. ما با استفاده از برنامه‌های شخصی‌سازی‌شده و پیگیری مستمر، به شما کمک می‌کنیم به اهداف بدنی‌تان برسید.</p>
            <div style="display:grid;gap:10px;margin-top:12px">
              <div class="program">
                <div class="icon">🔥</div>
                <div>
                  <h4 style="margin:0">HIIT & فیتنس</h4>
                  <p>چربی‌سوزی سریع با جلسات پرفشار اما کوتاه.</p>
                </div>
              </div>
              <div class="program">
                <div class="icon">💪</div>
                <div>
                  <h4 style="margin:0">بدنسازی حرفه‌ای</h4>
                  <p>پریودایزیشن، فرم صحیح و تغذیه مکمل.</p>
                </div>
              </div>
              <div class="program">
                <div class="icon">🧘‍♀️</div>
                <div>
                  <h4 style="margin:0">یوگا و ریکاوری</h4>
                  <p>افزایش انعطاف و کاهش آسیب با تمرینات اصلاحی.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Programs -->
  <section id="programs">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">برنامه‌ها و خدمات</h3>
          <p class="subtitle">پکیج مناسب هدفت را انتخاب کن</p>
        </div>
        <div class="chip">مشاوره رایگان</div>
      </div>
      <div class="grid">
        <div class="card col-4">
          <img src="https://images.unsplash.com/photo-1599050751795-5f7fdbdfe9c5?q=80&w=2069&auto=format&fit=crop" alt="تمرین قدرتی">
          <div class="card-body">
            <h4>قدرتی (Strength)</h4>
            <p class="subtitle">تمرکز بر افزایش قدرت و حجم عضلات با برنامه‌های علمی.</p>
          </div>
        </div>
        <div class="card col-4">
          <img src="https://images.unsplash.com/photo-1518314916381-77a37c2a49ae?q=80&w=2069&auto=format&fit=crop" alt="کلاس گروهی">
          <div class="card-body">
            <h4>کلاس‌های گروهی</h4>
            <p class="subtitle">زومبا، HIIT، کراس‌فیت و بیشتر — انرژی گروه را حس کن!</p>
          </div>
        </div>
        <div class="card col-4">
          <img src="https://images.unsplash.com/photo-1549060279-7e168fcee0c2?q=80&w=2069&auto=format&fit=crop" alt="مشاوره تغذیه">
          <div class="card-body">
            <h4>تغذیه و فالوآپ</h4>
            <p class="subtitle">پلن غذایی شخصی‌سازی‌شده و پیگیری ماهانه.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Trainers -->
  <section id="trainers">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">مربیان ما</h3>
          <p class="subtitle">تیمی از متخصصان با مدارک معتبر</p>
        </div>
        <div class="chip">+10 مربی</div>
      </div>
      <div class="grid">
        <div class="card col-6"><div class="card-body trainer"><img src="https://images.unsplash.com/photo-1556157382-97eda2d62296?q=80&w=1974&auto=format&fit=crop" alt="مربی ۱"><div><h4>آرش حیدری</h4><p class="subtitle">بدنسازی پیشرفته • مربی رسمی IFBB</p></div></div></div>
        <div class="card col-6"><div class="card-body trainer"><img src="https://images.unsplash.com/photo-1594737625785-c6683fc3690f?q=80&w=1974&auto=format&fit=crop" alt="مربی ۲"><div><h4>مریم کاویانی</h4><p class="subtitle">کاهش وزن • تمرینات اصلاحی</p></div></div></div>
        <div class="card col-6"><div class="card-body trainer"><img src="https://images.unsplash.com/photo-1584865288642-521e1b5216c0?q=80&w=1974&auto=format&fit=crop" alt="مربی ۳"><div><h4>پارسا یوسفی</h4><p class="subtitle">کراس‌فیت • آمادگی جسمانی</p></div></div></div>
        <div class="card col-6"><div class="card-body trainer"><img src="https://images.unsplash.com/photo-1558611848-73f7eb4001a1?q=80&w=1974&auto=format&fit=crop" alt="مربی ۴"><div><h4>نیلوفر مقدم</h4><p class="subtitle">یوگا • انعطاف و ریکاوری</p></div></div></div>
      </div>
    </div>
  </section>

  <!-- Pricing -->
  <section id="pricing">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">طرح‌ها و قیمت‌ها</h3>
          <p class="subtitle">انتخاب انعطاف‌پذیر، پرداخت آسان</p>
        </div>
        <div class="chip">پرداخت آنلاین/حضوری</div>
      </div>
      <div class="pricing">
        <div class="card price-card">
          <span class="badge chip">اقتصادی</span>
          <div class="card-body">
            <h4>ماهیانه</h4>
            <div class="price">۴۹۹٬۰۰۰ تومان</div>
            <ul class="features">
              <li>✓ دسترسی کامل به سالن</li>
              <li>✓ ۱ جلسه برنامه تمرینی</li>
              <li>— بدون کلاس گروهی</li>
            </ul>
            <a class="btn" href="#signup">انتخاب طرح</a>
          </div>
        </div>
        <div class="card price-card" style="border:1px solid rgba(244,63,94,.5)">
          <span class="badge chip" style="background:linear-gradient(135deg,var(--primary),#fb7185)">پیشنهادی</span>
          <div class="card-body">
            <h4>سه‌ماهه</h4>
            <div class="price">۱٬۳۹۹٬۰۰۰ تومان</div>
            <ul class="features">
              <li>✓ دسترسی کامل + کلاس‌های گروهی</li>
              <li>✓ ۳ جلسه مشاوره تغذیه</li>
              <li>✓ پیگیری هفتگی</li>
            </ul>
            <a class="btn primary" href="#signup">انتخاب طرح</a>
          </div>
        </div>
        <div class="card price-card">
          <span class="badge chip" style="background:linear-gradient(135deg,#22c55e,#16a34a)">حرفه‌ای</span>
          <div class="card-body">
            <h4>شخصی‌سازی</h4>
            <div class="price">تماس بگیرید</div>
            <ul class="features">
              <li>✓ برنامه اختصاصی با مربی خصوصی</li>
              <li>✓ جلسات اصلاحی و ریکاوری</li>
              <li>✓ اپلیکیشن پیگیری</li>
            </ul>
            <a class="btn" href="#contact">مشاهده جزئیات</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">گالری تصاویر</h3>
          <p class="subtitle">نگاهی به فضای باشگاه و کلاس‌ها</p>
        </div>
        <div class="chip">به‌روز می‌شود</div>
      </div>
      <div class="gallery" id="galleryGrid">
        <a href="#" data-src="https://images.unsplash.com/photo-1605296867304-46d5465a13f1?q=80&w=2030&auto=format&fit=crop"><img src="https://images.unsplash.com/photo-1605296867304-46d5465a13f1?q=80&w=900&auto=format&fit=crop" alt="وزنه آزاد"></a>
        <a href="#" data-src="https://images.unsplash.com/photo-1517963879433-6ad2b056d712?q=80&w=2030&auto=format&fit=crop"><img src="https://images.unsplash.com/photo-1517963879433-6ad2b056d712?q=80&w=900&auto=format&fit=crop" alt="تردمیل"></a>
        <a href="#" data-src="https://images.unsplash.com/photo-1596357395105-c9a3b95f0f05?q=80&w=2030&auto=format&fit=crop"><img src="https://images.unsplash.com/photo-1596357395105-c9a3b95f0f05?q=80&w=900&auto=format&fit=crop" alt="کراس‌فیت"></a>
        <a href="#" data-src="https://images.unsplash.com/photo-1526506118085-60ce8714f8c5?q=80&w=2030&auto=format&fit=crop"><img src="https://images.unsplash.com/photo-1526506118085-60ce8714f8c5?q=80&w=900&auto=format&fit=crop" alt="یوگا"></a>
      </div>
      <div id="lightbox" class="lightbox" role="dialog" aria-label="نمایش تصویر"><img alt="" src=""><span class="btn" id="closeLightbox" style="position:absolute;top:24px;left:24px">بستن ✕</span></div>
    </div>
  </section>

  <!-- Blog -->
  <section id="blog" class="blog">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">وبلاگ</h3>
          <p class="subtitle">نکات تمرینی و تغذیه‌ای از مربیان ما</p>
        </div>
        <a class="btn" href="#">مشاهده همه مقالات</a>
      </div>
      <div class="grid">
        <article class="card col-4"><img src="https://images.unsplash.com/photo-1604480133080-602261a680bf?q=80&w=2069&auto=format&fit=crop" alt="پروتئین و عضله سازی"><div class="card-body"><h4>چقدر پروتئین نیاز داریم؟</h4><div class="meta"><span>تغذیه</span><span>•</span><span>۵ دقیقه مطالعه</span></div><p class="subtitle">راهنمای سریع محاسبه پروتئین روزانه برای اهداف مختلف.</p><a class="btn" href="#">ادامه مطلب</a></div></article>
        <article class="card col-4"><img src="https://images.unsplash.com/photo-1517832606299-7ae9b720a186?q=80&w=2069&auto=format&fit=crop" alt="ریکاوری"><div class="card-body"><h4>اهمیت خواب و ریکاوری</h4><div class="meta"><span>تمرین</span><span>•</span><span>۴ دقیقه</span></div><p class="subtitle">چطور با ریکاوری هوشمندانه پیشرفت را چند برابر کنیم.</p><a class="btn" href="#">ادامه مطلب</a></div></article>
        <article class="card col-4"><img src="https://images.unsplash.com/photo-1597074866923-cf6c4c6b27f3?q=80&w=2069&auto=format&fit=crop" alt="HIIT"><div class="card-body"><h4>HIIT برای چربی‌سوزی سریع</h4><div class="meta"><span>کلاس‌ها</span><span>•</span><span>۳ دقیقه</span></div><p class="subtitle">نمونه یک جلسه ۲۰ دقیقه‌ای موثر و علمی.</p><a class="btn" href="#">ادامه مطلب</a></div></article>
      </div>
    </div>
  </section>

  <!-- Contact & Signup -->
  <section id="contact">
    <div class="container">
      <div class="head">
        <div>
          <h3 class="title">تماس با ما</h3>
          <p class="subtitle">ساعت کاری: همه‌روزه ۶ صبح تا ۱۱ شب</p>
        </div>
        <div class="chip">پارکینگ • رختکن • دوش</div>
      </div>

      <div class="contact-grid">
        <div class="card">
          <div class="card-body">
            <h4 id="signup">ثبت‌نام آنلاین</h4>
            <p class="subtitle">فرم زیر را پر کن؛ همکاران ما با شما تماس می‌گیرند.</p>
            <form id="signupForm">
              <div class="form-row">
                <input name="fullname" placeholder="نام و نام خانوادگی" required>
                <input name="mobile" placeholder="شماره موبایل" inputmode="tel" required>
              </div>
              <div class="form-row">
                <select name="plan" required>
                  <option value="monthly">طرح ماهیانه</option>
                  <option value="quarter">طرح سه‌ماهه (پیشنهادی)</option>
                  <option value="personal">مربی خصوصی</option>
                </select>
                <select name="time">
                  <option value="morning">صبح</option>
                  <option value="noon">ظهر</option>
                  <option value="evening">عصر</option>
                </select>
              </div>
              <textarea name="note" rows="4" placeholder="توضیحات (اختیاری)"></textarea>
              <label class="note"><input type="checkbox" required> قوانین باشگاه را می‌پذیرم.</label>
              <button class="btn primary" type="submit">ارسال درخواست</button>
              <div id="signupMsg" class="note"></div>
            </form>

            <div style="margin-top:18px;display:grid;gap:6px">
              <div>📍 آدرس: تهران، خیابان مثال، کوچه نمونه، پلاک ۱۲</div>
              <div>☎️ ۰۲۱-۱۲۳۴۵۶۷۸</div>
              <div>📧 info@fitnesspro.ir</div>
              <div style="display:flex;gap:10px;margin-top:6px">
                <a class="btn" href="#">اینستاگرام</a>
                <a class="btn" href="#">واتساپ</a>
                <a class="btn" href="#">تلگرام</a>
              </div>
            </div>
          </div>
        </div>
        <div class="map">
          <!-- Embed map: Replace with your Google Map iframe -->
          <iframe title="نقشه باشگاه" src="https://maps.google.com/maps?q=Tehran&t=&z=13&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" frameborder="0" style="filter:grayscale(40%) contrast(110%)"></iframe>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <div class="container" style="display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap">
      <div>© <span id="year"></span> FitnessPro — همه حقوق محفوظ است.</div>
      <div class="note">طراحی با عشق ✦</div>
    </div>
  </footer>

  <script>
    // Smooth scroll for internal links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click',e=>{ const id=a.getAttribute('href'); if(id.length>1){ e.preventDefault(); document.querySelector(id)?.scrollIntoView({behavior:'smooth'}); }});
    });

    // Trial form (Hero)
    const trialForm=document.getElementById('trialForm');
    trialForm?.addEventListener('submit',e=>{
      e.preventDefault();
      const form=new FormData(trialForm);
      const name=form.get('name');
      const phone=form.get('phone');
      const msg=document.getElementById('trialMsg');
      if(!/^\d{8,15}$/.test(String(phone).replace(/\D/g,''))){
        msg.textContent='لطفاً شماره تماس معتبر وارد کنید.';
        msg.style.color='var(--warn)';
        return;
      }
      msg.textContent='درخواست شما ثبت شد! همکاران ما به زودی تماس می‌گیرند.';
      msg.style.color='var(--ok)';
      trialForm.reset();
    });

    // Signup form (Contact)
    const signupForm=document.getElementById('signupForm');
    signupForm?.addEventListener('submit',e=>{
      e.preventDefault();
      const form=new FormData(signupForm);
      const mobile=String(form.get('mobile')||'').replace(/\D/g,'');
      const msg=document.getElementById('signupMsg');
      if(!/^\d{8,15}$/.test(mobile)){
        msg.textContent='شماره موبایل معتبر نیست.';
        msg.style.color='var(--warn)';
        return;
      }
      // Here you can POST to your backend / Google Sheet
      msg.textContent='درخواست با موفقیت ارسال شد. از تماس شما خوشحالیم!';
      msg.style.color='var(--ok)';
      signupForm.reset();
    });

    // Lightbox for gallery
    const lightbox=document.getElementById('lightbox');
    const lightImg=lightbox.querySelector('img');
    document.getElementById('galleryGrid').addEventListener('click',e=>{
      const a=e.target.closest('a');
      if(!a) return;
      e.preventDefault();
      lightImg.src=a.dataset.src;
      lightbox.style.display='grid';
    });
    document.getElementById('closeLightbox').addEventListener('click',()=>{lightbox.style.display='none';lightImg.src='';});
    lightbox.addEventListener('click',e=>{ if(e.target===lightbox){ lightbox.style.display='none'; lightImg.src=''; }});

    // Year
    document.getElementById('year').textContent=new Date().getFullYear();
  </script>
</body>
</html>
