<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfolio Hosting</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #0d1117;
      color: #ffffff;
      margin: 0;
      padding: 0;
      text-align: center;
    }

    .container {
      max-width: 600px;
      margin: 40px auto;
      padding: 20px;
      background-color: #161b22;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0, 255, 255, 0.2);
      animation: fadeInUp 1s ease-out; /* Animasi saat buka web */
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(40px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .logo-ring {
      position: relative;
      width: 200px;
      height: 200px;
      margin: 0 auto 20px;
      cursor: pointer;
    }

    .profile-img {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      border: 4px solid #00ffff;
      object-fit: cover;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 3;
    }

    .tech-logo {
      position: absolute;
      width: 40px;
      height: 40px;
      border-radius: 50%;
      opacity: 0;
      transform: scale(0) translate(-50%, -50%);
      transition: 0.5s ease;
    }

    .tech-logo.show {
      opacity: 1;
      transform: scale(1) translate(-50%, -50%);
      animation: swingUp 0.6s ease;
    }

    .tech-logo img {
      width: 100%;
      border-radius: 50%;
    }

    @keyframes swingUp {
      0% { transform: scale(0) translate(-50%, -50%) rotate(0deg); }
      50% { transform: scale(1.1) translate(-50%, -60%) rotate(10deg); }
      100% { transform: scale(1) translate(-50%, -50%) rotate(0); }
    }

    h1 {
      color: #00ffff;
      margin-top: 20px;
    }

    .desc {
      font-size: 16px;
      margin: 20px auto;
      color: #cccccc;
    }

    .product {
      background-color: #222;
      border: 2px solid #00ffff;
      border-radius: 10px;
      margin: 15px auto;
      padding: 15px;
      width: 90%;
      max-width: 400px;
      transition: 0.3s;
    }

    .product:hover {
      transform: scale(1.03);
      box-shadow: 0 0 10px #00ffff;
    }

    .product a {
      color: #00ffff;
      font-size: 18px;
      font-weight: bold;
      text-decoration: none;
    }

    .product-desc {
      margin-top: 5px;
      font-size: 14px;
      color: #aaa;
    }

    .social-media {
      margin-top: 30px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px;
    }

    .social-media a {
      padding: 8px 15px;
      background-color: #222;
      border: 2px solid #00ffff;
      border-radius: 8px;
      color: #00ffff;
      font-weight: bold;
      text-decoration: none;
      transition: 0.3s;
      font-size: 14px;
    }

    .social-media a:hover {
      transform: scale(1.05);
      background-color: #00ffff;
      color: #0d1117;
    }
  </style>
</head>
<body>

  <div class="container">
    <!-- Logo Ring dengan Foto Profil -->
    <div class="logo-ring" onclick="toggleLogos()">
      <img class="profile-img" src="https://files.catbox.moe/xm0r9r.jpg" alt="Foto Profil">

      <!-- Logo Teknologi -->
      <div class="tech-logo" style="top: 0%; left: 50%;" id="logo1">
        <img src="https://cdn-icons-png.flaticon.com/512/919/919827.png" title="HTML">
      </div>
      <div class="tech-logo" style="top: 25%; left: 90%;" id="logo2">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968350.png" title="Python">
      </div>
      <div class="tech-logo" style="top: 75%; left: 90%;" id="logo3">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968292.png" title="JavaScript">
      </div>
      <div class="tech-logo" style="top: 100%; left: 50%;" id="logo4">
        <img src="https://cdn-icons-png.flaticon.com/512/919/919830.png" title="PHP">
      </div>
      <div class="tech-logo" style="top: 75%; left: 10%;" id="logo5">
        <img src="https://files.catbox.moe/xm0r9r.jpg" title="SQL">
      </div>
      <div class="tech-logo" style="top: 25%; left: 10%;" id="logo6">
        <img src="https://cdn-icons-png.flaticon.com/512/6132/6132222.png" title="C++">
      </div>
    </div>

    <h1>Ziddy Hosting</h1>
    <div class="desc">
      Layanan hosting terbaik untuk kebutuhan digitalmu.
    </div>

    <!-- Produk Hosting -->
    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+join+murbug+min+zid" target="_blank">MURBUG PREMIUM 10k</a>
      <div class="product-desc">MENGUNAKAN SC IMPROVE V13 PRO YG PASTI NYA GACOR, DAN ANTI NYOLONG DI CH</div>
    </div>

    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+join+mursun+min+zid" target="_blank">MURSUN 5k</a>
      <div class="product-desc">BEBAS SUNTIK SOSMED SEPERTI TIKTOK, INSTAGRAM, YOUTUBE</div>
    </div>

    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+join+marga+SC+min+zid" target="_blank">MARGA SC 35k</a>
      <div class="product-desc">PEMBUATAN SC SECARA MANUAL DAN TIDAK MEMBUAT MENGGUNAKAN BOT</div>
    </div>

    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+order+jasa+suntik+min+zid" target="_blank">SUNTIK ALL SOSMED</a>
      <div class="product-desc">UNTUK MENAMBAH FOLLOWERS, LIKE, KOMEN</div>
    </div>

    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+join+admin+ch+min+zid" target="_blank">ADMIN CH 15k</a>
      <div class="product-desc">BISA BEBAS JUALAN APA SAJA SEPERTI MURBUG,PANEL,RESELLER PANEL DAN TIDAK BOLEH PROMOSI JUDOL</div>
    </div>

    <div class="product">
      <a href="https://wa.me/6282258021692?text=+mau+order+jasa+rename+sc+min+zid" target="_blank">RENAME SC 55k</a>
      <div class="product-desc">BEBAS REQUEST MAU RENAME SEPERTI APA SAJA</div>
    </div>

    <div class="product">
      <a href="https://files.catbox.moe/m75znz.png" target="_blank">PENCET UNTUK KE QRIS ALL PAY</a>
      <div class="product-desc">PENCET SAJA</div>
    </div>

    <!-- Sosial Media -->
    <div class="social-media">
      <a href="https://www.instagram.com/ziddy_mods">Instagram</a>
      <a href="https://wa.me/6282258021692">WhatsApp</a>
      <a href="https://youtube.com/@ziddy_mods">YouTube</a>
      <a href="https://www.tiktok.com/@ziddysoftspoken">TikTok</a>
    </div>
  </div>

  <script>
    let logoShown = false;
    function toggleLogos() {
      for (let i = 1; i <= 6; i++) {
        const logo = document.getElementById("logo" + i);
        if (!logoShown) {
          setTimeout(() => {
            logo.classList.add("show");
          }, i * 150);
        } else {
          logo.classList.remove("show");
        }
      }
      logoShown = !logoShown;
    }
  </script>

</body>
</html>
