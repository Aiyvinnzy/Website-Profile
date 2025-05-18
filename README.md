
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Profile Davin Zulfan X-3</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet" />
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(-45deg, #a3c9f1, #b9d7e8, #dbe9f4, #c6def6);
      background-size: 400% 400%;
      animation: gradientAnimation 30s ease infinite;
      color: #ffffff;
      text-align: center;
      transition: background-color 0.5s ease;
      position: relative;
      overflow-x: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(255, 255, 255, 0.15);
      pointer-events: none;
      z-index: 0;
    }

    @keyframes gradientAnimation {
      0% {
        background-position: 0% 50%;
      }
      50% {
        background-position: 100% 50%;
      }
      100% {
        background-position: 0% 50%;
      }
    }

    .marquee {
      background-color: white;
      color: #3498db;
      padding: 15px 0;
      font-size: 26px;
      font-weight: 600;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
      position: relative;
      z-index: 1;
    }

    .container {
      margin-top: 60px;
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
      z-index: 1;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
      padding: 0 15px;
    }

    img.clickable {
      width: 200px; /* Ukuran gambar diperkecil */
      height: auto;
      margin: 25px;
      cursor: pointer;
      border-radius: 16px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      border: 2px solid white;
      position: relative;
      z-index: 1;
    }

    img.clickable:hover {
      transform: scale(1.05);
      box-shadow: 0 12px 25px rgba(0, 0, 0, 0.2);
    }

    .bio {
      position: relative;
      padding: 20px 25px;
      background: rgba(255, 255, 255, 0.15);
      border-radius: 15px;
      box-shadow: 0 8px 15px rgba(0,0,0,0.1);
      text-align: justify;
      color: #000000cc;
      font-weight: 300;
      line-height: 1.5;
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
      margin-bottom: 80px;
    }

    .bio p {
      margin-bottom: 1em;
    }

    .instagram-logo {
      width: 90px;
      height: 90px;
      position: absolute;
      bottom: -60px;
      left: 15px;
      cursor: pointer;
      transition: transform 0.3s ease;
      background: rgba(255,255,255,0.7);
      border-radius: 50%;
      padding: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }

    .instagram-logo:hover {
      transform: scale(1.2);
      background: rgba(255,255,255,0.9);
    }

    a {
      text-decoration: none;
    }

    .footer {
      margin-top: 60px;
      font-size: 14px;
      color: rgba(0, 0, 0, 0.7);
      position: relative;
      z-index: 1;
    }   
  </style>
</head>
<body>

  <div class="marquee">
    <marquee>Selamat datang di Profile Davin Zulfan!</marquee>
  </div>

  <div class="container">
    <!-- Gambar PNG yang diklik untuk memutar audio -->
    <img
      src="https://i.imgur.com/EsZUZOs.jpg"
      alt="Klik untuk mendengar suara"
      class="clickable"
      onclick="playAudio()"
    />

    <div class="bio">
      <p>Halo semuanya, perkenalkan nama saya Davin Zulfan. Saya lahir pada 21 Maret 2009 di Jakarta, dan saat ini bersekolah di SMAN 27 Jakarta. Saya memiliki beberapa hobi yang cukup menarik, di antaranya adalah saya suka membaca buku baik itu fiksi maupun nonfiksi, lalu saya juga suka bermain basket dan bermain game. Saya memiliki cita-cita untuk bisa menjadi IT/Programmer karena saya yakin di masa depan nanti ilmu inilah yang akan sangat berguna, maka dari itu saya ingin mempelajari lebih dalam tentang materi ini untuk mempersiapkan masa depan saya.</p>

      <p>Saya orangnya juga sangat suka berpetualang atau menjelajahi tempat baru karena bagi saya itu bisa menambah ilmu dan pengetahuan baru akan luasnya dunia ini yang dipenuhi dengan berbagai macam budaya. Saya juga sangat suka jika ada orang yang menceritakan bagaimana luasnya dunia ini ataupun jika ada orang yang tertarik dengan cerita saya. Nah, biasanya jika saya memiliki waktu luang, saya sempatkan untuk membaca manga ataupun menonton anime terbaru karena sebetulnya itu juga termasuk dalam hobi saya. Mungkin ini saja biodata singkat dari saya.</p>

      <p class="footer">Terima kasih.</p>

      <!-- Instagram link -->
      <a href="https://www.instagram.com/vinnzy.zyy/" target="_blank" rel="noopener noreferrer" title="Instagram Davin Zulfan">
        <img
          src="https://upload.wikimedia.org/wikipedia/commons/e/e7/Instagram_logo_2016.svg"
          alt="Instagram"
          class="instagram-logo"
        />
      </a>
    </div>
  </div>

  <!-- Audio -->
  <audio id="voiceAudio" src="Recording (6).mp3"></audio>

  <div class="footer">
    &copy; 2025 Davin Zulfan
  </div>

  <script>
    function playAudio() {
      const audio = document.getElementById('voiceAudio');
      audio.play();
    }
  </script>

</body>
</html>
