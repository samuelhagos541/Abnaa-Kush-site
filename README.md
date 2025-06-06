<html lang="ar">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>فريق ابناء كوش للعبادة و التسبيح</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@600;800&family=Inter:wght@500;700&display=swap" rel="stylesheet">
  <!-- Tailwind CDN for utility classes -->
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .font-cairo-custom { font-family: 'Cairo', 'Segoe UI', 'Arial', 'Noto Naskh Arabic', serif; }
    .font-inter-custom { font-family: 'Inter', 'Cairo', 'Segoe UI', Arial, sans-serif; }
    @keyframes fadeInBox {
      0% { opacity: 0; transform: scale(0.94) translateY(10px);}
      100% { opacity: 1; transform: scale(1) translateY(0);}
    }
    .animate-main-box {
      animation: fadeInBox 1.3s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
    }
    @keyframes pulseGlow {
      0% { text-shadow: 0 2px 12px #8b0000aa; }
      50% { text-shadow: 0 2px 20px #8b0000dd, 0 0 30px #ff4d4daa; }
      100% { text-shadow: 0 2px 12px #8b0000aa; }
    }
    .animate-pulse-glow {
      animation: pulseGlow 2.5s infinite ease-in-out;
      animation-delay: 1.5s;
    }
    @keyframes iconPopIn {
      0% { opacity: 0; transform: scale(0.3) translateY(20px);}
      60% { opacity: 1; transform: scale(1.1) translateY(-5px);}
      100% { opacity: 1; transform: scale(1) translateY(0);}
    }
    .animate-icon-pop-in {
      animation-name: iconPopIn;
      animation-duration: 0.6s;
      animation-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55);
      animation-fill-mode: forwards;
      opacity: 0;
      transform: scale(0.3);
    }
    .social-icon-transition {
      transition: transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1), box-shadow 0.3s cubic-bezier(0.34, 1.56, 0.64, 1), border-color 0.3s ease-out, filter 0.3s ease-out;
    }
    .socials a:active {
      transform: scale(0.95) translateY(0px) !important;
      box-shadow: 0 2px 10px #1976d233 !important;
      filter: brightness(90%) saturate(100%) !important;
      transition-duration: 0.1s;
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(5px); }
      100% { opacity: 1; transform: translateY(0); }
    }
    .animate-fade-in {
      animation: fadeIn 2s 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
    }
    @media (max-width: 540px) {
      .main-box-responsive {
        padding: 25px 5vw 20px 5vw;
        border-radius: 12px;
      }
      .title-line1 { font-size: 1.19em !important; }
      .title-line2 { font-size: 0.95em !important; }
    }
  </style>
</head>
<body class="m-0 min-h-screen bg-[#b3e0ff] text-[#222] flex justify-center items-center h-screen overflow-x-hidden relative">
  <div class="main-box bg-[#e6f7ff] rounded-[18px] shadow-[0_8px_36px_#1976d240,0_1.5px_8px_#8b000044] px-5 py-10 text-center max-w-[420px] w-[90%] flex flex-col items-center opacity-0 transform scale-[0.94] translate-y-[10px] main-box-responsive" id="main-content">
    <div class="main-title rtl font-cairo-custom font-extrabold mb-2 text-[#1d3557] animate-pulse-glow">
      <div class="title-line1 text-[2.1em] mb-[0.1em] tracking-tight">فريق ابناء كوش</div>
      <div class="title-line2 text-[1.15em] text-[#1976d2] font-semibold mt-0 tracking-wider">للعبادة و التسبيح</div>
    </div>
    <div class="follow-us text-[1.15em] text-[#222] mb-5 rtl font-cairo-custom font-semibold animate-pulse-glow">تابعونا على منصات التواصل الاجتماعي</div>
    <div class="socials flex justify-center gap-5 my-3 flex-wrap">
      <a href="https://www.instagram.com/abnaa.kush/" target="_blank" title="Instagram" aria-label="Instagram" class="group flex items-center justify-center w-14 h-14 rounded-full bg-white shadow-[0_3px_15px_#1976d233] social-icon-transition border-[2.5px] border-[#b3e0ff] relative overflow-hidden hover:scale-112 hover:translate-y-[-8px] hover:rotate-[-5deg] hover:shadow-[0_20px_40px_#1976d2aa,0_5px_20px_#8b000066] hover:border-[#1976d2] hover:brightness-120 hover:saturate-150">
        <svg class="social-icon w-[30px] h-[30px] block transition-transform duration-250 ease-out group-hover:scale-115" viewBox="0 0 50 50">
          <defs>
            <radialGradient id="ig" cx="0.35" cy="0.95" r="1.5">
              <stop offset="0%" stop-color="#fdf497"/>
              <stop offset="25%" stop-color="#fd5949"/>
              <stop offset="50%" stop-color="#d6249f"/>
              <stop offset="100%" stop-color="#285AEB"/>
            </radialGradient>
            <filter id="instagram-shadow">
              <feDropShadow dx="0" dy="2" stdDeviation="2" flood-color="#000" flood-opacity="0.3"/>
            </filter>
          </defs>
          <path d="M25 4.5 A 20.5 20.5 0 1 0 25 45.5 A 20.5 20.5 0 1 0 25 4.5 Z" fill="url(#ig)" filter="url(#instagram-shadow)"/>
          <path d="M25 12.5 A 12.5 12.5 0 1 0 25 37.5 A 12.5 12.5 0 1 0 25 12.5 Z" fill="none" stroke="#fff" stroke-width="2.5"/>
          <path d="M25 17.5 A 7.5 7.5 0 1 0 25 32.5 A 7.5 7.5 0 1 0 25 17.5 Z" fill="none" stroke="#fff" stroke-width="2.5"/>
          <circle cx="34" cy="16" r="2.5" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.facebook.com/profile.php?id=61561245110328" target="_blank" title="Facebook" aria-label="Facebook" class="group flex items-center justify-center w-14 h-14 rounded-full bg-white shadow-[0_3px_15px_#1976d233] social-icon-transition border-[2.5px] border-[#b3e0ff] relative overflow-hidden hover:scale-112 hover:translate-y-[-8px] hover:rotate-[5deg] hover:shadow-[0_20px_40px_#1976d2aa,0_5px_20px_#8b000066] hover:border-[#1976d2] hover:brightness-120 hover:saturate-150">
        <svg class="social-icon w-[30px] h-[30px] block transition-transform duration-250 ease-out group-hover:scale-115" viewBox="0 0 50 50">
          <defs>
            <linearGradient id="fb-gradient" x1="0%" y1="0%" x2="0%" y2="100%">
              <stop offset="0%" stop-color="#1877F3"/>
              <stop offset="100%" stop-color="#0F67DA"/>
            </linearGradient>
            <filter id="facebook-shadow">
              <feDropShadow dx="0" dy="2" stdDeviation="2" flood-color="#000" flood-opacity="0.3"/>
            </filter>
          </defs>
          <circle cx="25" cy="25" r="22" fill="url(#fb-gradient)" filter="url(#facebook-shadow)"/>
          <path d="M29 38V26h4l1-6h-5v-3c0-1.7.6-3 2.4-3H34V9.5C33.4 9.4 32 9 30.3 9 26.4 9 24 11.1 24 15v5h-4v6h4v12h6z" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.tiktok.com/@abnaakush8" target="_blank" title="TikTok" aria-label="TikTok" class="group flex items-center justify-center w-14 h-14 rounded-full bg-white shadow-[0_3px_15px_#1976d233] social-icon-transition border-[2.5px] border-[#b3e0ff] relative overflow-hidden hover:scale-112 hover:translate-y-[-8px] hover:rotate-[-5deg] hover:shadow-[0_20px_40px_#1976d2aa,0_5px_20px_#8b000066] hover:border-[#1976d2] hover:brightness-120 hover:saturate-150">
        <svg class="social-icon w-[30px] h-[30px] block transition-transform duration-250 ease-out group-hover:scale-115" viewBox="0 0 50 50">
          <defs>
            <radialGradient id="tiktok-gradient" cx="50%" cy="50%" r="50%" fx="60%" fy="40%">
              <stop offset="0%" stop-color="#333"/>
              <stop offset="100%" stop-color="#000"/>
            </radialGradient>
            <filter id="tiktok-shadow">
              <feDropShadow dx="0" dy="2" stdDeviation="2" flood-color="#000" flood-opacity="0.4"/>
            </filter>
          </defs>
          <circle cx="25" cy="25" r="22" fill="url(#tiktok-gradient)" filter="url(#tiktok-shadow)"/>
          <path d="M32.5 18.5c1.7 0 3.2-.7 4.3-1.7v4.3c-1.3.1-2.6-.1-3.8-.5v8.7c0 4.6-3.7 8.3-8.3 8.3s-8.3-3.7-8.3-8.3 3.7-8.3 8.3-8.3v4.1c-2.3 0-4.2 1.9-4.2 4.2 0 2.3 1.9 4.2 4.2 4.2 2.3 0 4.2-1.9 4.2-4.2V13.2c1.1.7 2.4 1.3 3.8 1.3z" fill="#fff"/>
          <path d="M36.8 16.8c-1.1 1-2.7 1.7-4.3 1.7-1.4 0-2.7-.6-3.8-1.3v2c1.2.4 2.5.6 3.8.5v-2.9c1.1.7 2.4 1.3 3.8 1.3v-1.3h.5z" fill="#25F4EE"/>
          <path d="M28.7 11.5v17.8c0 2.3-1.9 4.2-4.2 4.2s-4.2-1.9-4.2-4.2c0-2.3 1.9-4.2 4.2-4.2v-2c-4.6 0-8.3 3.7-8.3 8.3s3.7 8.3 8.3 8.3 8.3-3.7 8.3-8.3V12.8c-1.4-.3-2.7-.8-3.8-1.3z" fill="#FE2C55"/>
        </svg>
      </a>
      <a href="https://m.youtube.com/@abnaakush4081" target="_blank" title="YouTube" aria-label="YouTube" class="group flex items-center justify-center w-14 h-14 rounded-full bg-white shadow-[0_3px_15px_#1976d233] social-icon-transition border-[2.5px] border-[#b3e0ff] relative overflow-hidden hover:scale-112 hover:translate-y-[-8px] hover:rotate-[5deg] hover:shadow-[0_20px_40px_#1976d2aa,0_5px_20px_#8b000066] hover:border-[#1976d2] hover:brightness-120 hover:saturate-150">
        <svg class="social-icon w-[30px] h-[30px] block transition-transform duration-250 ease-out group-hover:scale-115" viewBox="0 0 50 50">
          <defs>
            <radialGradient id="youtube-gradient" cx="50%" cy="50%" r="50%" fx="60%" fy="40%">
              <stop offset="0%" stop-color="#FF0000"/>
              <stop offset="100%" stop-color="#CC0000"/>
            </radialGradient>
            <filter id="youtube-shadow">
              <feDropShadow dx="0" dy="2" stdDeviation="2" flood-color="#000" flood-opacity="0.3"/>
            </filter>
          </defs>
          <circle cx="25" cy="25" r="22" fill="url(#youtube-gradient)" filter="url(#youtube-shadow)"/>
          <polygon points="20,17 37,25 20,33" fill="#fff"/>
        </svg>
      </a>
    </div>
    <div class="footer text-[#1976d2] bg-[#1976d212] rounded-lg mt-7 mx-auto max-w-[340px] px-4 py-2.5 text-[0.97em] animate-fade-in opacity-0 font-inter-custom">
      © 2025 فريق ابناء كوش للعبادة و التسبيح. جميع الحقوق محفوظة.
    </div>
  </div>
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const mainContent = document.getElementById('main-content');
      const socialLinks = document.querySelectorAll('.socials a');
      mainContent.classList.add('animate-main-box');
      mainContent.style.opacity = '1';
      socialLinks.forEach((link, index) => {
        setTimeout(() => {
          link.classList.add('animate-icon-pop-in');
        }, index * 100);
      });
      // Footer fade-in
      setTimeout(() => {
        document.querySelector('.footer').style.opacity = '1';
      }, 1100);
    });
  </script>
</body>
</html>
