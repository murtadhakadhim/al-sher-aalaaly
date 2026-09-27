<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>شركة الشراع العالي للمقاولات العامة المحدودة</title>
<meta name="description" content="حلول متكاملة في المقاولات العامة والإنشاءات والأعمال الهندسية والبنية التحتية في العراق.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans+Arabic:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --brand-primary:#1b3a63;
  --brand-secondary:#2a5a9c;
  --brand-accent:#009688;
  --brand-dark:#0a1220;
  --brand-light:#f2f5f8;
  --brand-white:#ffffff;
  --brand-gray:#7c8a9a;
  --background:#fafbfc;
  --foreground:var(--brand-dark);
  --muted:#eef1f4;
  --muted-foreground:#5c6a78;
  --border:#dbe1e7;
  --shadow:0 10px 30px rgba(10,18,32,0.08);
  --transition:all 0.3s ease;
}

*{box-sizing:border-box;border-color:var(--border);margin:0;padding:0}
html{scroll-behavior:smooth}
body{
  background:var(--background);
  color:var(--foreground);
  font-family:"IBM Plex Sans Arabic",sans-serif;
  overflow-x:hidden;
  line-height:1.6;
}
a{color:inherit;text-decoration:none}
button, input, textarea{font:inherit}

/* Layout Utility */
.container{width:min(100% - 48px, 1280px);margin-inline:auto}
.pad{padding-block:clamp(60px, 8vw, 110px)}

/* Navigation */
.header{
  position:fixed;
  top:0;
  right:0;
  left:0;
  z-index:1000;
  background:rgba(255,255,255,0.95);
  backdrop-filter:blur(10px);
  border-bottom:1px solid var(--border);
  box-shadow:0 2px 10px rgba(0,0,0,0.03);
}
.nav-container{
  display:flex;
  align-items:center;
  justify-content:space-between;
  height:80px;
}
.logo{
  display:flex;
  align-items:center;
  gap:12px;
  font-weight:700;
  font-size:1.35rem;
  color:var(--brand-primary);
}
.logo-icon{
  width:42px;
  height:42px;
  background:var(--brand-primary);
  color:var(--brand-white);
  border-radius:8px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:1.4rem;
}
.nav-links{
  display:flex;
  gap:28px;
  list-style:none;
}
.nav-links a{
  font-weight:500;
  color:var(--muted-foreground);
  transition:var(--transition);
}
.nav-links a:hover{
  color:var(--brand-primary);
}
.btn{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:12px 26px;
  border-radius:6px;
  font-weight:600;
  transition:var(--transition);
  cursor:pointer;
  border:none;
}
.btn-primary{
  background:var(--brand-primary);
  color:var(--brand-white);
}
.btn-primary:hover{
  background:var(--brand-secondary);
  transform:translateY(-2px);
}
.btn-outline{
  border:2px solid var(--brand-white);
  color:var(--brand-white);
}
.btn-outline:hover{
  background:var(--brand-white);
  color:var(--brand-primary);
}

/* Hero Section */
.hero{
  position:relative;
  min-height:90vh;
  display:flex;
  align-items:center;
  padding-top:80px;
  background:linear-gradient(135deg, rgba(27,58,99,0.92), rgba(10,18,32,0.95)), url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.04'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
  color:var(--brand-white);
}
.hero-content{
  max-width:780px;
}
.hero-tag{
  display:inline-block;
  background:rgba(255,255,255,0.15);
  padding:6px 16px;
  border-radius:30px;
  font-size:0.9rem;
  margin-bottom:20px;
  letter-spacing:0.5px;
}
.hero h1{
  font-size:clamp(2.4rem, 5vw, 3.8rem);
  font-weight:700;
  line-height:1.2;
  margin-bottom:24px;
}
.hero p{
  font-size:1.25rem;
  color:rgba(255,255,255,0.85);
  margin-bottom:36px;
  max-width:650px;
}
.hero-btns{
  display:flex;
  gap:16px;
  flex-wrap:wrap;
}

/* Stats Section */
.stats-bar{
  background:var(--brand-white);
  border-radius:12px;
  box-shadow:var(--shadow);
  margin-top:-60px;
  position:relative;
  z-index:10;
  padding:32px;
  display:grid;
  grid-template-columns:repeat(auto-fit, minmax(200px, 1fr));
  gap:24px;
  text-align:center;
}
.stat-item h3{
  font-size:2.4rem;
  color:var(--brand-primary);
  font-weight:700;
  margin-bottom:4px;
}
.stat-item p{
  color:var(--muted-foreground);
  font-size:0.95rem;
}

/* Section Header */
.section-header{
  text-align:center;
  max-width:650px;
  margin:0 auto 50px auto;
}
.section-header span{
  color:var(--brand-secondary);
  font-weight:600;
  text-transform:uppercase;
  font-size:0.9rem;
  letter-spacing:1px;
}
.section-header h2{
  font-size:2.2rem;
  color:var(--brand-dark);
  margin-top:8px;
}

/* Services */
.services-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit, minmax(300px, 1fr));
  gap:30px;
}
.service-card{
  background:var(--brand-white);
  padding:36px 28px;
  border-radius:10px;
  border:1px solid var(--border);
  transition:var(--transition);
}
.service-card:hover{
  transform:translateY(-6px);
  box-shadow:var(--shadow);
  border-color:var(--brand-secondary);
}
.service-icon{
  width:56px;
  height:56px;
  background:var(--brand-light);
  color:var(--brand-primary);
  border-radius:8px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:1.8rem;
  margin-bottom:20px;
}
.service-card h3{
  font-size:1.3rem;
  margin-bottom:12px;
  color:var(--brand-dark);
}
.service-card p{
  color:var(--muted-foreground);
  font-size:0.98rem;
  line-height:1.7;
}

/* About Section */
.about{
  background:var(--brand-light);
}
.about-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:50px;
  align-items:center;
}
.about-text h2{
  font-size:2.2rem;
  color:var(--brand-dark);
  margin-bottom:20px;
}
.about-text p{
  color:var(--muted-foreground);
  margin-bottom:20px;
  line-height:1.8;
}
.about-list{
  list-style:none;
  margin-top:20px;
}
.about-list li{
  display:flex;
  align-items:center;
  gap:10px;
  margin-bottom:12px;
  font-weight:600;
  color:var(--brand-primary);
}

/* Projects */
.projects-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit, minmax(320px, 1fr));
  gap:30px;
}
.project-card{
  background:var(--brand-white);
  border-radius:10px;
  overflow:hidden;
  border:1px solid var(--border);
  box-shadow:0 4px 15px rgba(0,0,0,0.03);
}
.project-img{
  height:220px;
  background:linear-gradient(135deg, var(--brand-secondary), var(--brand-dark));
  display:flex;
  align-items:center;
  justify-content:center;
  color:var(--brand-white);
  font-size:3rem;
}
.project-info{
  padding:24px;
}
.project-info h3{
  font-size:1.25rem;
  margin-bottom:8px;
}
.project-info p{
  color:var(--muted-foreground);
  font-size:0.95rem;
}

/* Contact Section */
.contact-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:40px;
}
.contact-form{
  background:var(--brand-white);
  padding:36px;
  border-radius:12px;
  border:1px solid var(--border);
  box-shadow:var(--shadow);
}
.form-group{
  margin-bottom:20px;
}
.form-group label{
  display:block;
  margin-bottom:8px;
  font-weight:500;
  color:var(--brand-dark);
}
.form-control{
  width:100%;
  padding:12px 16px;
  border:1px solid var(--border);
  border-radius:6px;
  outline:none;
  transition:var(--transition);
}
.form-control:focus{
  border-color:var(--brand-primary);
}
.contact-info-card{
  background:var(--brand-primary);
  color:var(--brand-white);
  padding:40px;
  border-radius:12px;
  display:flex;
  flex-direction:column;
  justify-content:space-between;
}
.info-item{
  margin-bottom:24px;
}
.info-item h4{
  font-size:1.1rem;
  margin-bottom:6px;
  opacity:0.85;
}
.info-item p{
  font-size:1.15rem;
  font-weight:500;
}

/* Footer */
footer{
  background:var(--brand-dark);
  color:var(--brand-white);
  padding-block:50px 30px;
  border-top:1px solid rgba(255,255,255,0.1);
}
.footer-container{
  display:flex;
  justify-content:space-between;
  align-items:center;
  flex-wrap:wrap;
  gap:20px;
}
.footer-copy{
  color:var(--brand-gray);
  font-size:0.9rem;
}

@media (max-width: 768px){
  .nav-links{display:none;}
  .about-grid, .contact-grid{grid-template-columns:1fr;}
  .hero h1{font-size:2rem;}
}
</style>
</head>
<body>

  <!-- Header / Navigation -->
  <header class="header">
    <div class="container nav-container">
      <a href="#" class="logo">
        <div class="logo-icon">🏗️</div>
        <span>الشراع العالي</span>
      </a>
      <ul class="nav-links">
        <li><a href="#home">الرئيسية</a></li>
        <li><a href="#about">من نحن</a></li>
        <li><a href="#services">خدماتنا</a></li>
        <li><a href="#projects">مشاريعنا</a></li>
        <li><a href="#contact">تواصل معنا</a></li>
      </ul>
      <a href="#contact" class="btn btn-primary">تواصل معنا</a>
    </div>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <div class="container">
      <div class="hero-content">
        <span class="hero-tag">شركة الشراع العالي للمقاولات العامة المحدودة</span>
        <h1>نموّ بثبات.. ونبني المستقبل بمعايير عالمية</h1>
        <p>نحن متفوقون في تقديم حلول هندسية وإنشائية متكاملة في العراق، معتمدين على الخبرة والابتكار وأعلى معايير الجودة والسلامة.</p>
        <div class="hero-btns">
          <a href="#services" class="btn btn-primary">استكشف خدماتنا</a>
          <a href="#contact" class="btn btn-outline">طلب استشارة</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Stats Bar -->
  <div class="container">
    <div class="stats-bar">
      <div class="stat-item">
        <h3>+15</h3>
        <p>سنة من الخبرة</p>
      </div>
      <div class="stat-item">
        <h3>+120</h3>
        <p>مشروع منجز</p>
      </div>
      <div class="stat-item">
        <h3>100%</h3>
        <p>التزام بالمعايير</p>
      </div>
      <div class="stat-item">
        <h3>+50</h3>
        <p>مهندس واستشاري</p>
      </div>
    </div>
  </div>

  <!-- About Section -->
  <section id="about" class="pad about">
    <div class="container">
      <div class="about-grid">
        <div class="about-text">
          <h2>عن شركة الشراع العالي</h2>
          <p>تُعد شركة الشراع العالي للمقاولات العامة المحدودة واحدة من الشركات الوطنية الرائدة في مجال الانشاءات والبنية التحتية والاستشارات الهندسية في جمهورية العراق.</p>
          <p>تسعى الشركة دائماً إلى تنفيذ المشاريع الإنشائية والهندسية بأعلى كفاءة وبأحدث التقنيات المتاحة مع مراعاة كافة السلامة البيئية والمهنية.</p>
          <ul class="about-list">
            <li>✓ التزام صارم بجدول التنفيذ والتعاقدات</li>
            <li>✓ فريق عمل متكامل من أمهر المهندسين والخبراء</li>
            <li>✓ تطبيق معايير الجودة الشاملة في كافة المراحل</li>
          </ul>
        </div>
        <div class="about-card" style="background: var(--brand-primary); color: white; padding: 40px; border-radius: 12px;">
          <h3 style="font-size: 1.8rem; margin-bottom: 16px;">رؤيتنا ورسالتنا</h3>
          <p style="opacity: 0.9; margin-bottom: 20px; line-height: 1.8;">أن نكون الخيار الأول في قطاع المقاولات والبناء في المنطقة عبر تقديم مشاريع مستدامة تسهم بشكل فعال في بناء وتطوير البنية التحتية.</p>
          <div style="border-top: 1px solid rgba(255,255,255,0.2); padding-top: 20px;">
            <p style="font-weight: 600;">القيم الأساسية:</p>
            <p style="opacity: 0.85;">النزاهة، الكفاءة، الابتكار، والسلامة المهنية.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="pad">
    <div class="container">
      <div class="section-header">
        <span>مجالات عملنا</span>
        <h2>الخدمات التي نقدمها</h2>
      </div>
      <div class="services-grid">
        <div class="service-card">
          <div class="service-icon">🏢</div>
          <h3>المقاولات العامة والإنشاءات</h3>
          <p>بناء وتشييد المجمعات السكنية، والمباني التجارية، والمؤوسسات الحكومية والمرافق العامة بكفاءة عالية.</p>
        </div>
        <div class="service-card">
          <div class="service-icon">🛣️</div>
          <h3>مشاريع البنية التحتية</h3>
          <p>تنفيذ وتطوير شبكات الطرق، والجسور، وشبكات المياه والفرز الصحي وفق أحدث المخططات الهندسية.</p>
        </div>
        <div class="service-card">
          <div class="service-icon">⚙️</div>
          <h3>الأعمال الكهروميكانيكية</h3>
          <p>تجهيز وتركيب كافة الأنظمة الكهربائية والميكانيكية والتكييف المركزي للمشاريع الضخمة.</p>
        </div>
        <div class="service-card">
          <div class="service-icon">📐</div>
          <h3>التصاميم والاستشارات الهندسية</h3>
          <p>إعداد الدراسات الفنية والتصاميم المبتكرة وإدارة المشاريع لضمان أقصى درجات الجودة.</p>
        </div>
        <div class="service-card">
          <div class="service-icon">🛠️</div>
          <h3>الصيانة والتأهيل</h3>
          <p>ترميم وإعادة تأهيل المباني والمنشآت القائمة وتحديث بنيتها التحتية باستمرار.</p>
        </div>
        <div class="service-card">
          <div class="service-icon">🚜</div>
          <h3>تأجير المعدات الآلية</h3>
          <p>توظيف وتأمين أحدث الآليات والمعدات الثقيلة للمشاريع الإنشائية والصناعية المختلفة.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="pad" style="background:var(--brand-light)">
    <div class="container">
      <div class="section-header">
        <span>سجل النجاحات</span>
        <h2>أبرز مشاريعنا</h2>
      </div>
      <div class="projects-grid">
        <div class="project-card">
          <div class="project-img">🏢</div>
          <div class="project-info">
            <h3>مجمع سكني متكامل</h3>
            <p>تشييد وتنفيذ مجمع سكني حديث بجميع المرافق الخدمية والبنية التحتية.</p>
          </div>
        </div>
        <div class="project-card">
          <div class="project-img">🌉</div>
          <div class="project-info">
            <h3>تطوير البنية التحتية والطرق</h3>
            <p>مشروع مد وتعبيد الطرق الرئيسية وتطوير شبكات صرف المياه.</p>
          </div>
        </div>
        <div class="project-card">
          <div class="project-img">🏛️</div>
          <div class="project-info">
            <h3>مبنى إداري وتجاري</h3>
            <p>تنفيذ مشروع مبنى استثماري وتجاري وفق أعلى معايير الجودة المعمارية.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="pad">
    <div class="container">
      <div class="section-header">
        <span>تواصل معنا</span>
        <h2>نحن هنا لمساعدتك في مشروعك القادم</h2>
      </div>
      <div class="contact-grid">
        <form class="contact-form" onsubmit="event.preventDefault(); alert('شكراً لتواصلك معنا! سنرد عليك في أسرع وقت ممكن.');">
          <div class="form-group">
            <label>الاسم الكامل</label>
            <input type="text" class="form-control" placeholder="أدخل اسمك" required>
          </div>
          <div class="form-group">
            <label>البريد الإلكتروني</label>
            <input type="email" class="form-control" placeholder="example@domain.com" required>
          </div>
          <div class="form-group">
            <label>رقم الهاتف</label>
            <input type="tel" class="form-control" placeholder="+964 7XX XXX xXXX" required>
          </div>
          <div class="form-group">
            <label>تفاصيل المشروع / الرسالة</label>
            <textarea class="form-control" rows="4" placeholder="اكتب تفاصيل استفسارك هنا..." required></textarea>
          </div>
          <button type="submit" class="btn btn-primary" style="width: 100%;">إرسال الطلب</button>
        </form>

        <div class="contact-info-card">
          <div>
            <h3>معلومات الاتصال</h3>
            <p style="margin-top: 10px; opacity: 0.85;">يسعدنا استقبال استفساراتكم وزيارتكم في مقر الشركة الرئيسي.</p>
          </div>
          
          <div>
            <div class="info-item">
              <h4>العنوان</h4>
              <p>بغداد، جمهورية العراق</p>
            </div>
            <div class="info-item">
              <h4>البريد الإلكتروني</h4>
              <p>info@alshiraa-alali.com</p>
            </div>
            <div class="info-item">
              <h4>الهاتف</h4>
              <p>+964 770 000 0000</p>
            </div>
          </div>

          <div>
            <p style="font-size: 0.9rem; opacity: 0.7;">أوقات العمل: الأحد - الخميس (8:00 صباحاً - 4:00 مساءً)</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container footer-container">
      <div class="logo" style="color:var(--brand-white)">
        <span>شركة الشراع العالي للمقاولات العامة المحدودة</span>
      </div>
      <p class="footer-copy">جميع الحقوق محفوظة © 2026 شركة الشراع العالي للمقاولات العامة المحدودة.</p>
    </div>
  </footer>

</body>
</html>