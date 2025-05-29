<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>Abnaa Kush</title>
  <style>
    body {
      margin: 0;
      min-height: 100vh;
      background: linear-gradient(135deg, #444 0%, #aaa 100%);
      /* dark silver gradient */
      color: #e0e0e0;
      font-family: 'Segoe UI', sans-serif;
      transition: background 1s;
    }
    .glow-red {
      box-shadow: 0 0 32px 0 #8b0000cc, 0 4px 24px 0 #60010399;
      transition: box-shadow 0.6s;
    }
    h1, .subtitle {
      text-align: center;
      font-size: 2.4em;
      color: #fff;
      text-shadow: 0 4px 16px #8b0000cc;
      margin-top: 30px;
      animation: fadeInDown 1.2s ease;
    }
    @keyframes fadeInDown {
      0% { opacity: 0; transform: translateY(-60px); }
      100% { opacity: 1; transform: translateY(0); }
    }
    .mission {
      background: rgba(34,34,34,0.85);
      color: #fff;
      border-radius: 12px;
      margin: 24px auto;
      max-width: 600px;
      padding: 18px 28px 20px 28px;
      box-shadow: 0 0 24px #8b000099;
      font-size: 1.2em;
      animation: fadeIn 2s;
    }
    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    .socials {
      display: flex;
      justify-content: center;
      gap: 22px;
      margin: 32px 0;
      animation: bounceIn 1.4s;
    }
    @keyframes bounceIn {
      0% { opacity: 0; transform: scale(0.7);}
      60% { opacity: 1; transform: scale(1.1);}
      100% { opacity: 1; transform: scale(1);}
    }
    .socials a img {
      filter: drop-shadow(0 0 10px #8b0000cc);
      transition: transform 0.3s, filter 0.3s;
    }
    .socials a:hover img {
      transform: scale(1.15) rotate(-5deg);
      filter: drop-shadow(0 0 24px #a80000);
    }
    .contact {
      text-align: center;
      margin-top: 12px;
      font-size: 1.1em;
      color: #ffb4b4;
      animation: fadeIn 2.5s;
    }
    .footer {
      text-align: center;
      color: #aaa;
      background: rgba(50,10,10,0.18);
      border-radius: 8px;
      margin: 24px auto 0 auto;
      max-width: 460px;
      padding: 10px 0;
      font-size: 1em;
      box-shadow: 0 3px 18px #8b000077;
      animation: fadeIn 3s;
    }
  </style>
</head>
<body>
  <h1 class="subtitle glow-red">Praise & Worship Team<br><span style="font-size:0.7em;">فريق أبناء كوش العبادة والتسبيح</span></h1>
  <div class="mission glow-red">
    <strong style="color:#e63946;">Our Mission:</strong><br>
    To be filled with a deep knowledge of biblical truth to share the message of Christ with Sudanese people everywhere through songs and media content using various communication tools, and by building a strong community rooted in love and hope.
  </div>
  <div class="socials">
    <a href="https://www.instagram.com/abnaa.kush/" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" height="40" alt="Instagram"></a>
    <a href="https://www.facebook.com/profile.php?id=61561245110328" target="_blank"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" height="40" alt="Facebook"></a>
    <a href="https://www.tiktok.com/@abnaakush8" target="_blank"><img src="https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white" height="40" alt="TikTok"></a>
    <a href="https://youtube.com/@abnaakush4081?feature=shared" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" height="40" alt="YouTube"></a>
  </div>
  <div class="contact">
    📧 <a href="mailto:abnaakushworshipteam@gmail.com" style="color:#38bdf8; text-decoration:underline;">abnaakushworshipteam@gmail.com</a>
  </div>
  <div class="footer">
    &copy; 2025 Abnaa Kush. All rights reserved.
  </div>
</body>
</html>
