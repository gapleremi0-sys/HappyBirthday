# HappyBirthday
<!DOCTYPE html><html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>HBD Ferdy Ayu Febryyanty 🎉</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Comic Sans MS', 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ffd6e8, #fff1c1);
      overflow: hidden;
    }
    .page {
      display: none;
      min-height: 100vh;
      padding: 40px 20px;
      text-align: center;
      animation: fade 1s ease;
    }
    .page.active { display: block; }
    h1 { color: #ff5fa2; font-size: 2.2rem; }
    h2 { color: #ff7eb3; }
    p { font-size: 1.1rem; line-height: 1.6; }
    .btn {
      margin-top: 25px;
      padding: 12px 25px;
      background: #ff7eb3;
      color: white;
      border: none;
      border-radius: 25px;
      font-size: 1rem;
      cursor: pointer;
      box-shadow: 0 6px 15px rgba(0,0,0,0.2);
    }
    .btn:hover { transform: scale(1.05); }/* dekorasi */
.decor {
  font-size: 2rem;
  animation: float 3s ease-in-out infinite;
}

/* kucing */
.cat {
  font-size: 4rem;
  animation: catJump 1.2s infinite alternate;
  margin: 20px 0;
}

@keyframes fade {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
@keyframes float {
  0% { transform: translateY(0); }
  50% { transform: translateY(-15px); }
  100% { transform: translateY(0); }
}
@keyframes catJump {
  from { transform: translateY(0); }
  to { transform: translateY(-20px); }
}

  </style>
</head>
<body>  <!-- PAGE 1 -->  <div class="page active">
    <div class="decor">🎈✨🎂✨🎈</div>
    <h1>Hai Ferdy Ayu Febryyanty 💖</h1>
    <div class="cat">🐱</div>
    <p>Hari ini bukan hari biasa… karena kamu GENAP 17 TAHUN 🎉</p>
    <button class="btn" onclick="nextPage()">Lanjut 👉</button>
  </div>  <!-- PAGE 2 -->  <div class="page">
    <h1>Sweet Seventeen 💫</h1>
    <div class="cat">🐈‍⬛</div>
    <p>17 tahun itu umur yang cantik 🌸<br>
    Semoga kamu makin bahagia, makin kuat, dan makin percaya diri ✨</p>
    <p class="decor">💐🌈💖</p>
    <button class="btn" onclick="nextPage()">Lanjut 👉</button>
  </div>  <!-- PAGE 3 -->  <div class="page">
    <h1>Doa Imut Untuk Kamu 🤍</h1>
    <div class="cat">🐱‍👓</div>
    <p>Semoga langkahmu selalu ringan,<br>
    senyummu selalu tulus,<br>
    dan hatimu selalu dikelilingi orang baik 🫶</p>
    <p class="decor">⭐🍰⭐</p>
    <button class="btn" onclick="nextPage()">Lanjut 👉</button>
  </div>  <!-- PAGE 4 -->  <div class="page">
    <h1>Kamu Itu Spesial 🥰</h1>
    <div class="cat">🐈</div>
    <p>Terima kasih sudah menjadi versi dirimu yang hangat 🌷<br>
    Jangan ragu untuk bermimpi besar ya ✨</p>
    <p class="decor">🎀🧁🎀</p>
    <button class="btn" onclick="nextPage()">Lanjut 👉</button>
  </div>  <!-- PAGE 5 -->  <div class="page">
    <h1>Selamat Ulang Tahun 🎊</h1>
    <div class="cat">🐱🎉</div>
    <p>Selamat ulang tahun ke-17<br>
    <strong>Ferdy Ayu Febryyanty</strong> 💕<br><br>
    Semoga semua harapan baikmu satu per satu terwujud 🤍</p>
    <p class="decor">🎂🎈🎉</p>
    <button class="btn" onclick="alert('🎉 HAPPY BIRTHDAY 17 🎉')">Peluk Virtual 🤗</button>
  </div>  <script>
    let current = 0;
    const pages = document.querySelectorAll('.page');

    function nextPage() {
      pages[current].classList.remove('active');
      current = (current + 1) % pages.length;
      pages[current].classList.add('active');
    }
  </script></body>
</html>
