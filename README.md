<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tentang Safika 💫</title>

  <style>
    /* 🎨 STYLE DASAR */
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #a1c4fd, #c2e9fb);
      color: #333;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      flex-direction: column;
      overflow-x: hidden;
    }

    h1 {
      font-size: 2.5rem;
      color: #2b2d42;
      animation: fadeInDown 1s ease forwards;
    }

    h2 {
      color: #1a759f;
      margin-bottom: 0.5em;
    }

    p {
      line-height: 1.6;
    }

    /* 📦 CONTAINER */
    .card {
      background: #fff;
      padding: 30px 40px;
      border-radius: 15px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
      width: 80%;
      max-width: 700px;
      animation: slideUp 1.2s ease;
    }

    ul {
      list-style: none;
      padding: 0;
    }

    ul li::before {
      content: "🌸 ";
    }

    /* 🌈 ANIMASI */
    @keyframes fadeInDown {
      0% { opacity: 0; transform: translateY(-30px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      0% { opacity: 0; transform: translateY(50px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    /* 🔗 LINK */
    a {
      color: #1a759f;
      text-decoration: none;
      font-weight: 600;
      transition: 0.3s;
    }

    a:hover {
      color: #457b9d;
      text-decoration: underline;
    }

    /* ✨ QUOTE */
    blockquote {
      margin-top: 20px;
      font-style: italic;
      color: #555;
      border-left: 4px solid #1a759f;
      padding-left: 10px;
      animation: fadeInDown 1.5s ease;
    }

    /* 💫 EFEK TEKS BERGERAK */
    .typewriter {
      overflow: hidden;
      border-right: .15em solid #1a759f;
      white-space: nowrap;
      animation: typing 3.5s steps(30, end), blink-caret .75s step-end infinite;
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }

    @keyframes blink-caret {
      from, to { border-color: transparent }
      50% { border-color: #1a759f; }
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>💫 Halo, Aku Safikha Nur Hikmah!</h1>
    <p class="typewriter">Biasa dipanggil Safika atau Fika 👋</p>

    <h2>🌱 Tentang Saya</h2>
    <ul>
      <li>💻 Siswi kelas 11 jurusan RPL (Rekayasa Perangkat Lunak)</li>
      <li>🎧 Hobi: mendengarkan musik, menonton film, dan memanjat pohon 🌳</li>
      <li>✨ Suka mencoba hal baru, terutama yang berhubungan dengan teknologi</li>
    </ul>

    <h2>📫 Kontak</h2>
    <p>
      💬 Instagram: <a href="https://instagram.com/usernamekamu" target="_blank">@usernamekamu</a><br>
      📧 Email: <a href="mailto:yourname@email.com">yourname@email.com</a>
    </p>

    <h2>🚀 Tujuan Saya</h2>
    <p>Saya ingin menjadi seorang <strong>programmer handal</strong> dan membuat aplikasi yang bermanfaat bagi banyak orang!</p>

    <blockquote>“Setiap baris kode adalah langkah kecil menuju mimpi besar.” ✨</blockquote>
  </div>

  <script>
    // 🎉 Animasi tambahan: bintang jatuh di background
    const createStar = () => {
      const star = document.createElement('div');
      star.classList.add('star');
      star.style.left = Math.random() * 100 + 'vw';
      star.style.animationDuration = Math.random() * 2 + 3 + 's';
      document.body.append(star);

      setTimeout(() => star.remove(), 5000);
    }

    setInterval(createStar, 300);

    const style = document.createElement('style');
    style.innerHTML = `
      .star {
        position: fixed;
        top: 0;
        width: 2px;
        height: 10px;
        background: white;
        opacity: 0.8;
        animation: fall linear forwards;
      }
      @keyframes fall {
        to { transform: translateY(100vh); opacity: 0; }
      }
    `;
    document.head.appendChild(style);
  </script>

</body>
</html>
