<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>فريق ابناء كوش للعبادة و التسبيح</title>
  <!-- Google Fonts: Cairo (Arabic modern), Inter (English modern) -->
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@600;800&family=Inter:wght@500;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      min-height: 100vh;
      background: #b3e0ff;
      color: #222;
      font-family: 'Cairo', 'Inter', 'Segoe UI', Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .main-box {
      background: #e6f7ff;
      border-radius: 18px;
      box-shadow: 0 8px 36px #1976d240, 0 1.5px 8px #8b000044;
      padding: 40px 22px 28px 22px;
      text-align: center;
      max-width: 420px;
      width: 100%;
      animation: fadeInBox 1.3s;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    @keyframes fadeInBox {
      0% { opacity: 0; transform: scale(0.94);}
      100% { opacity: 1; transform: scale(1);}
    }
    .glow-red {
      text-shadow: 0 4px 18px #8b0000cc;
    }
    .main-title {
      direction: rtl;
      font-family: 'Cairo', 'Segoe UI', 'Arial', 'Noto Naskh Arabic', serif;
      font-weight: 800;
      margin-bottom: 8px;
      color: #1d3557;
    }
    .title-line1 {
      font-size: 2.1em;
      margin-bottom: 0.1em;
      letter-spacing: 0.01em;
    }
    .title-line2 {
      font-size: 1.15em;
      color: #1976d2;
      font-weight: 600;
      margin-top: 0;
      letter-spacing: 0.02em;
    }
    .follow-us {
      font-size: 1.15em;
      color: #222;
      margin-bottom: 18px;
      direction: rtl;
      font-family: 'Cairo', 'Segoe UI', 'Arial', 'Noto Naskh Arabic', serif;
      font-weight: 600;
    }
    .socials {
      display: flex;
      justify-content: center;
      gap: 16px;
      margin: 12px 0 2px 0;
      flex-wrap: wrap;
    }
    .socials a {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 48px;
      height: 48px;
      border-radius: 50%;
      background: #fff;
      box-shadow: 0 2px 12px #1976d233;
      transition: transform 0.26s, box-shadow 0.26s;
      border: 2px solid #b3e0ff;
      position: relative;
      overflow: hidden;
    }
    .socials a:hover {
      transform: scale(1.09) rotate(-4deg);
      box-shadow: 0 6px 20px #1976d277;
      border-color: #1976d2;
    }
    .social-icon {
      width: 26px;
      height: 26px;
      display: block;
    }
    .footer {
      color: #1976d2;
      background: rgba(50,10,10,0.05);
      border-radius: 8px;
      margin: 18px auto 0 auto;
      max-width: 340px;
      padding: 8px 0 0 0;
      font-size: 0.97em;
      animation: fadeIn 2s;
      font-family: 'Inter', 'Cairo', 'Segoe UI', Arial, sans-serif;
    }
    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    /* Responsive Design */
    @media (max-width: 540px) {
      body {
        padding: 0;
        height: auto;
        min-height: 100vh;
      }
      .main-box {
        margin: 0 0;
        padding: 22px 6vw 20px 6vw;
        max-width: 98vw;
        min-width: 0;
        border-radius: 10px;
      }
      .title-line1 {
        font-size: 1.19em;
      }
      .title-line2 {
        font-size: 0.95em;
      }
      .footer {
        max-width: 95vw;
        font-size: 0.93em;
      }
      .socials {
        gap: 10px;
      }
      .socials a {
        width: 40px;
        height: 40px;
      }
      .social-icon {
        width: 20px;
        height: 20px;
      }
    }
  </style>
</head>
<body>
  <div class="main-box">
    <div class="main-title glow-red">
      <div class="title-line1">فريق ابناء كوش</div>
      <div class="title-line2">للعبادة و التسبيح</div>
    </div>
    <div class="follow-us glow-red">تابعونا على منصات التواصل الاجتماعي</div>
    <div class="socials">
      <a href="https://www.instagram.com/abnaa.kush/" target="_blank" title="Instagram" aria-label="Instagram">
        <!-- Instagram SVG -->
        <svg class="social-icon" viewBox="0 0 50 50">
          <radialGradient id="ig" cx="0.5" cy="0.5" r="0.7">
            <stop offset="0%" stop-color="#fdf497"/>
            <stop offset="50%" stop-color="#fd5949"/>
            <stop offset="100%" stop-color="#d6249f"/>
          </radialGradient>
          <circle cx="25" cy="25" r="22" fill="url(#ig)"/>
          <rect x="12" y="12" width="26" height="26" rx="8" fill="none" stroke="#fff" stroke-width="3"/>
          <circle cx="25" cy="25" r="7" fill="none" stroke="#fff" stroke-width="2"/>
          <circle cx="33" cy="17" r="2" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.facebook.com/profile.php?id=61561245110328" target="_blank" title="Facebook" aria-label="Facebook">
        <!-- Facebook SVG -->
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#1877F3"/>
          <path d="M29 38V26h4l1-6h-5v-3c0-1.7.6-3 2.4-3H34V9.5C33.4 9.4 32 9 30.3 9 26.4 9 24 11.1 24 15v5h-4v6h4v12h6z" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.tiktok.com/@abnaakush8" target="_blank" title="TikTok" aria-label="TikTok">
        <!-- TikTok SVG -->
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#000"/>
          <path d="M32.5 18.5c1.7 0 3.2-.7 4.3-1.7v4.3c-1.3.1-2.6-.1-3.8-.5v8.7c0 4.6-3.7 8.3-8.3 8.3s-8.3-3.7-8.3-8.3 3.7-8.3 8.3-8.3v4.1c-2.3 0-4.2 1.9-4.2 4.2 0 2.3 1.9 4.2 4.2 4.2 2.3 0 4.2-1.9 4.2-4.2V13.2c1.1.7 2.4 1.3 3.8 1.3z" fill="#fff"/>
          <path d="M36.8 16.8c-1.1 1-2.7 1.7-4.3 1.7-1.4 0-2.7-.6-3.8-1.3v2c1.2.4 2.5.6 3.8.5v-2.9c1.1.7 2.4 1.3 3.8 1.3v-1.3h.5z" fill="#25F4EE"/>
          <path d="M28.7 11.5v17.8c0 2.3-1.9 4.2-4.2 4.2s-4.2-1.9-4.2-4.2c0-2.3 1.9-4.2 4.2-4.2v-2c-4.6 0-8.3 3.7-8.3 8.3s3.7 8.3 8.3 8.3 8.3-3.7 8.3-8.3V12.8c-1.4-.3-2.7-.8-3.8-1.3z" fill="#FE2C55"/>
        </svg>
      </a>
      <a href="https://youtube.com/@abnaakush4081?feature=shared" target="_blank" title="YouTube" aria-label="YouTube">
        <!-- YouTube SVG -->
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#FF0000"/>
          <polygon points="20,17 37,25 20,33" fill="#fff"/>
        </svg>
      </a>
    </div>
    <div class="footer">
      &copy; 2025 فريق ابناء كوش للعبادة و التسبيح. جميع الحقوق محفوظة.
    </div>
  </div>
</body>
</html>
