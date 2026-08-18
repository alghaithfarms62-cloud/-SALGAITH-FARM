<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>الغيث | Alghaith Farms</title>
  <meta name="description" content="الغيث - مكانك المثالي للراحة والاستجمام وقضاء أجمل الأوقات وسط الطبيعة والهدوء.">

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background: #f5f3ed;
      color: #1f2a20;
      line-height: 1.7;
    }

    /* ===== HEADER ===== */

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(255,255,255,.95);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid #ddd;
    }

    nav {
      max-width: 1150px;
      height: 75px;
      margin: auto;
      padding: 0 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 26px;
      font-weight: bold;
      color: #315b3a;
      white-space: nowrap;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 25px;
    }

    nav a {
      text-decoration: none;
      color: #26372b;
      font-weight: bold;
    }

    nav a:hover {
      color: #b08427;
    }

    .menu-btn {
      display: none;
      background: none;
      border: none;
      font-size: 30px;
      cursor: pointer;
      color: #315b3a;
    }

    /* ===== HERO ===== */

    .hero {
      min-height: 100vh;
      background:
        linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.58)),
        url("https://images.unsplash.com/photo-1500534623283-312aade485b7?auto=format&fit=crop&w=2000&q=85")
        center/cover;

      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
      padding: 110px 20px 50px;
    }

    .hero-content {
      max-width: 800px;
    }

    .hero h1 {
      font-size: clamp(48px, 9vw, 85px);
      margin-bottom: 12px;
    }

    .hero p {
      font-size: clamp(18px, 3vw, 23px);
      margin-bottom: 32px;
    }

    .btn {
      display: inline-block;
      background: #d4a84f;
      color: white;
      padding: 14px 30px;
      border-radius: 12px;
      text-decoration: none;
      font-weight: bold;
      border: none;
      cursor: pointer;
      font-size: 17px;
      transition: .25s;
    }

    .btn:hover {
      transform: translateY(-2px);
      background: #bd9137;
    }

    /* ===== SECTIONS ===== */

    section {
      max-width: 1150px;
      margin: auto;
      padding: 90px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 45px;
    }

    .section-title h2 {
      font-size: 38px;
      color: #315b3a;
      margin-bottom: 8px;
    }

    .section-title p {
      color: #777;
    }

    /* ===== ABOUT ===== */

    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 45px;
      align-items: center;
    }

    .about img {
      width: 100%;
      height: 420px;
      object-fit: cover;
      border-radius: 25px;
    }

    .about-text h2 {
      color: #315b3a;
      font-size: 38px;
      margin-bottom: 15px;
    }

    .about-text p {
      color: #555;
      font-size: 18px;
    }

    /* ===== FEATURES ===== */

    .features {
      background: #fff;
      max-width: none;
    }

    .features-inner {
      max-width: 1150px;
      margin: auto;
    }

    .feature-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .feature {
      background: #f8f7f2;
      padding: 30px 20px;
      text-align: center;
      border-radius: 20px;
      transition: .25s;
    }

    .feature:hover {
      transform: translateY(-5px);
    }

    .feature-icon {
      font-size: 42px;
      margin-bottom: 12px;
    }

    .feature h3 {
      color: #315b3a;
      margin-bottom: 7px;
    }

    .feature p {
      color: #777;
      font-size: 15px;
    }

    /* ===== PLACES ===== */

    .cards {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .card {
      background: white;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 8px 30px rgba(0,0,0,.08);
      transition: .3s;
    }

    .card:hover {
      transform: translateY(-6px);
    }

    .card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .card-content {
      padding: 22px;
    }

    .card h3 {
      color: #315b3a;
      font-size: 23px;
      margin-bottom: 8px;
    }

    .card p {
      color: #666;
    }

    .price {
      color: #b08427;
      font-size: 21px;
      font-weight: bold;
      margin: 15px 0;
    }

    /* ===== BOOKING ===== */

    .booking {
      background: #315b3a;
      color: white;
      max-width: none;
    }

    .booking-inner {
      max-width: 900px;
      margin: auto;
    }

    .booking h2 {
      text-align: center;
      font-size: 38px;
      margin-bottom: 35px;
    }

    form {
      background: white;
      color: #222;
      padding: 30px;
      border-radius: 20px;
      display: grid;
      gap: 18px;
      box-shadow: 0 15px 40px rgba(0,0,0,.12);
    }

    label {
      font-weight: bold;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 14px;
      border: 1px solid #ddd;
      border-radius: 10px;
      font-size: 16px;
      margin-top: 6px;
      outline: none;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: #315b3a;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    .submit {
      background: #d4a84f;
      color: white;
      border: none;
      padding: 15px;
      border-radius: 10px;
      font-size: 18px;
      font-weight: bold;
      cursor: pointer;
    }

    .submit:hover {
      background: #bd9137;
    }

    .booking-note {
      text-align: center;
      margin-top: 15px;
      color: #eee;
      font-size: 14px;
    }

    /* ===== CONTACT ===== */

    .contact {
      text-align: center;
    }

    .contact-box {
      background: white;
      padding: 40px 25px;
      border-radius: 20px;
      box-shadow: 0 8px 30px rgba(0,0,0,.06);
    }

    .contact-box h3 {
      color: #315b3a;
      margin-bottom: 5px;
    }

    .contact-item {
      margin-bottom: 25px;
    }

    /* ===== FOOTER ===== */

    footer {
      background: #1d2c20;
      color: white;
      text-align: center;
      padding: 30px 20px;
    }

    footer strong {
      color: #d4a84f;
    }

    /* ===== MOBILE ===== */

    @media (max-width: 900px) {

      .feature-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .cards {
        grid-template-columns: 1fr;
      }

      .about {
        grid-template-columns: 1fr;
      }

      .about img {
        height: 330px;
      }
    }

    @media (max-width: 700px) {

      nav {
        height: 68px;
      }

      .logo {
        font-size: 23px;
      }

      .menu-btn {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 68px;
        right: 0;
        width: 100%;
        background: white;
        padding: 20px;
        flex-direction: column;
        gap: 18px;
        border-bottom: 1px solid #ddd;
      }

      .nav-links.active {
        display: flex;
      }

      .hero {
        min-height: 90vh;
      }

      .hero h1 {
        font-size: 52px;
      }

      .hero p {
        font-size: 18px;
      }

      section {
        padding: 70px 18px;
      }

      .section-title h2 {
        font-size: 31px;
      }

      .about-text h2 {
        font-size: 31px;
      }

      .feature-grid {
        grid-template-columns: 1fr 1fr;
        gap: 12px;
      }

      .feature {
        padding: 22px 12px;
      }

      form {
        padding: 22px;
      }
    }

    @media (max-width: 430px) {

      .feature-grid {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 45px;
      }

      .btn {
        width: 100%;
      }

      .card .btn {
        width: 100%;
        text-align: center;
      }
    }
  </style>
</head>

<body>

<!-- ===== HEADER ===== -->

<header>

  <nav>

    <div class="logo">
      🌿 الغيث
    </div>

    <button class="menu-btn" id="menuBtn">
      ☰
    </button>

    <div class="nav-links" id="navLinks">

      <a href="#home">الرئيسية</a>
      <a href="#about">عن الغيث</a>
      <a href="#features">المميزات</a>
      <a href="#places">الخانات</a>
      <a href="#booking">الحجز</a>
      <a href="#contact">تواصل معنا</a>

    </div>

  </nav>

</header>


<!-- ===== HERO ===== -->

<div class="hero" id="home">

  <div class="hero-content">

    <h1>الغيث</h1>

    <p>
      مكانك المثالي للراحة والاستجمام
      وقضاء أجمل الأوقات وسط الطبيعة والهدوء
    </p>

    <a href="#booking" class="btn">
      احجز الآن
    </a>

  </div>

</div>


<!-- ===== ABOUT ===== -->

<section id="about">

  <div class="about">

    <img
      src="https://images.unsplash.com/photo-1473448912268-2022ce9509d8?auto=format&fit=crop&w=1200&q=85"
      alt="الغيث">

    <div class="about-text">

      <h2>عن الغيث</h2>

      <p>
        أهلاً وسهلاً بكم في الغيث 🌿
      </p>

      <br>

      <p>
        مكان مصمم حتى تستمتع بأجواء هادئة
        وجميلة بعيداً عن ضوضاء المدينة،
        مع مساحات مريحة تناسب العوائل
        والأصدقاء.
      </p>

      <br>

      <p>
        هدفنا أن تكون زيارتكم للغيث
        تجربة جميلة تستحق التكرار.
      </p>

      <br>

      <a href="#places" class="btn">
        شوف الخانات
      </a>

    </div>

  </div>

</section>


<!-- ===== FEATURES ===== -->

<section class="features" id="features">

  <div class="features-inner">

    <div class="section-title">

      <h2>ليش تختار الغيث؟</h2>

      <p>
        كل شيء تحتاجه حتى تستمتع بيوم جميل
      </p>

    </div>

    <div class="feature-grid">

      <div class="feature">

        <div class="feature-icon">🌳</div>

        <h3>أجواء طبيعية</h3>

        <p>
          مكان هادئ بعيد عن الزحام
        </p>

      </div>


      <div class="feature">

        <div class="feature-icon">🏡</div>

        <h3>خانات خاصة</h3>

        <p>
          أماكن مناسبة للعوائل والأصدقاء
        </p>

      </div>


      <div class="feature">

        <div class="feature-icon">🏊</div>

        <h3>ترفيه واستجمام</h3>

        <p>
          مساحة مناسبة لقضاء يوم ممتع
        </p>

      </div>


      <div class="feature">

        <div class="feature-icon">👨‍👩‍👧‍👦</div>

        <h3>مناسب للعوائل</h3>

        <p>
          أجواء مريحة للجميع
        </p>

      </div>

    </div>

  </div>

</section>


<!-- ===== PLACES ===== -->

<section id="places">

  <div class="section-title">

    <h2>الخانات المتوفرة</h2>

    <p>
      اختار الخانة المناسبة إلك واحجز موعدك
    </p>

  </div>


  <div class="cards">


    <!-- الخانة الملكية -->

    <div class="card">

      <img
        src="https://images.unsplash.com/photo-1540541338287-41700207dee6?auto=format&fit=crop&w=1000&q=85"
        alt="الخانة الملكية">

      <div class="card-content">

        <h3>الخانة الملكية</h3>

        <p>
          خانة خاصة ومريحة، مناسبة للعوائل
          والجلسات الخاصة.
        </p>

        <div class="price">
          150,000 د.ع
        </div>

        <button
          class="btn"
          onclick="selectPlace('الخانة الملكية')">

          احجز هذه الخانة

        </button>

      </div>

    </div>


    <!-- الخانة العائلية -->

    <div class="card">

      <img
        src="https://images.unsplash.com/photo-1601918774946-25832a4be0d6?auto=format&fit=crop&w=1000&q=85"
        alt="الخانة العائلية">

      <div class="card-content">

        <h3>الخانة العائلية</h3>

        <p>
          مساحة واسعة ومناسبة للعوائل
          والمناسبات الصغيرة.
        </p>

        <div class="price">
          100,000 د.ع
        </div>

        <button
          class="btn"
          onclick="selectPlace('الخانة العائلية')">

          احجز هذه الخانة

        </button>

      </div>

    </div>


    <!-- خانة الأصدقاء -->

    <div class="card">

      <img
        src="https://images.unsplash.com/photo-1475483768296-6163e08872a1?auto=format&fit=crop&w=1000&q=85"
        alt="خانة الأصدقاء">

      <div class="card-content">

        <h3>خانة الأصدقاء</h3>

        <p>
          جلسة جميلة للأصدقاء والشباب
          مع أجواء طبيعية هادئة.
        </p>

        <div class="price">
          75,000 د.ع
        </div>

        <button
          class="btn"
          onclick="selectPlace('خانة الأصدقاء')">

          احجز هذه الخانة

        </button>

      </div>

    </div>


  </div>

</section>


<!-- ===== BOOKING ===== -->

<section class="booking" id="booking">

  <div class="booking-inner">

    <h2>
      احجز موعدك 📅
    </h2>

    <form id="bookingForm">


      <div>

        <label>
          الاسم الكامل
        </label>

        <input
          type="text"
          id="name"
          placeholder="اكتب اسمك"
          required>

      </div>


      <div>

        <label>
          رقم الهاتف
        </label>

        <input
          type="tel"
          id="phone"
          placeholder="07XXXXXXXXX"
          required>

      </div>


      <div>

        <label>
          اختار الخانة
        </label>

        <select id="place" required>

          <option value="">
            اختر الخانة
          </option>

          <option value="الخانة الملكية">
            الخانة الملكية
          </option>

          <option value="الخانة العائلية">
            الخانة العائلية
          </option>

          <option value="خانة الأصدقاء">
            خانة الأصدقاء
          </option>

        </select>

      </div>


      <div>

        <label>
          تاريخ الحجز
        </label>

        <input
          type="date"
          id="date"
          required>

      </div>


      <div>

        <label>
          وقت الحجز
        </label>

        <input
          type="time"
          id="time"
          required>

      </div>


      <div>

        <label>
          عدد الأشخاص
        </label>

        <input
          type="number"
          id="people"
          min="1"
          max="100"
          placeholder="عدد الأشخاص"
          required>

      </div>


      <div>

        <label>
          ملاحظات
        </label>

        <textarea
          id="notes"
          placeholder="أي ملاحظات إضافية..."></textarea>

      </div>


      <button
        type="submit"
        class="submit">

        إرسال طلب الحجز عبر واتساب

      </button>


    </form>

    <p class="booking-note">
      بعد الضغط على الزر سيتم فتح واتساب وإرسال تفاصيل طلب الحجز.
    </p>

  </div>

</section>


<!-- ===== CONTACT ===== -->

<section id="contact">

  <div class="contact">

    <div class="section-title">

      <h2>
        تواصل معنا
      </h2>

      <p>
        نحن جاهزون لاستقبال استفساراتكم وحجوزاتكم
      </p>

    </div>


    <div class="contact-box">

      <div class="contact-item">

        <h3>
          📞 الهاتف
        </h3>

        <p>
          07XXXXXXXXX
        </p>

      </div>


      <div class="contact-item">

        <h3>
          📍 الموقع
        </h3>

        <p>
          العراق
        </p>

      </div>


      <a
        href="#booking"
        class="btn">

        احجز الآن

      </a>

    </div>

  </div>

</section>


<!-- ===== FOOTER ===== -->

<footer>

  <p>
    © 2026 <strong>الغيث</strong> - جميع الحقوق محفوظة
  </p>

</footer>


<!-- ===== JAVASCRIPT ===== -->

<script>

  /* =========================
     قائمة الموبايل
  ========================= */

  const menuBtn =
    document.getElementById("menuBtn");

  const navLinks =
    document.getElementById("navLinks");


  menuBtn.addEventListener("click", function() {

    navLinks.classList.toggle("active");

  });


  document
    .querySelectorAll(".nav-links a")
    .forEach(function(link) {

      link.addEventListener("click", function() {

        navLinks.classList.remove("active");

      });

    });


  /* =========================
     اختيار الخانة
  ========================= */

  function selectPlace(placeName) {

    document
      .getElementById("place")
      .value = placeName;

    document
      .getElementById("booking")
      .scrollIntoView({
        behavior: "smooth"
      });

  }


  /* =========================
     منع التاريخ السابق
  ========================= */

  const dateInput =
    document.getElementById("date");


  const today =
    new Date();


  const year =
    today.getFullYear();


  const month =
    String(today.getMonth() + 1)
      .padStart(2, "0");


  const day =
    String(today.getDate())
      .padStart(2, "0");


  const todayString =
    `${year}-${month}-${day}`;


  dateInput.min =
    todayString;


  /* =========================
     إرسال الحجز للواتساب
  ========================= */

  document
    .getElementById("bookingForm")
    .addEventListener("submit", function(e) {

      e.preventDefault();


      const name =
        document.getElementById("name").value.trim();


      const phone =
        document.getElementById("phone").value.trim();


      const place =
        document.getElementById("place").value;


      const date =
        document.getElementById("date").value;


      const time =
        document.getElementById("time").value;


      const people =
        document.getElementById("people").value;


      const notes =
        document.getElementById("notes").value.trim();


      /*
        مهم جداً:
        غيّر الرقم أدناه إلى رقم واتساب الغيث.

        مثال العراق:
        9647XXXXXXXXX

        بدون +
        وبدون الصفر الأول.
      */

      const whatsappNumber =
        "9647XXXXXXXXX";


      const message =
        `🌿 *طلب حجز - الغيث*

👤 الاسم: ${name}

📞 الهاتف: ${phone}

🏡 الخانة: ${place}

📅 التاريخ: ${date}

⏰ الوقت: ${time}

👥 عدد الأشخاص: ${people}

📝 الملاحظات: ${notes || "لا توجد ملاحظات"}

أرغب بتأكيد الحجز.`;

      
      const url =
        "https://wa.me/" +
        whatsappNumber +
        "?text=" +
        encodeURIComponent(message);


      window.open(
        url,
        "_blank"
      );

    });

</script>

</body>
</html>
