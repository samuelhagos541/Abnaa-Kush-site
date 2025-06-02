<html lang="ar">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>فريق ابناء كوش للعبادة و التسبيح</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@600;800&family=Inter:wght@500;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      min-height: 100vh;
      background: #b3e0ff; /* Light sky blue background */
      color: #222; /* Dark text color for readability */
      font-family: 'Cairo', 'Inter', 'Segoe UI', Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh; /* Full viewport height */
      overflow-x: hidden; /* Prevent horizontal scroll during animations */
      position: relative; /* Needed for absolute positioning of spinner */
    }
    .main-box {
      background: #e6f7ff; /* Very light blue, almost white, for the content box */
      border-radius: 18px; /* Rounded corners */
      box-shadow: 0 8px 36px #1976d240, 0 1.5px 8px #8b000044; /* Softer blue shadow and subtle red undertone shadow */
      padding: 40px 22px 28px 22px;
      text-align: center;
      max-width: 420px; /* Max width of the content box */
      width: 90%; /* Use percentage for better responsiveness, max-width will cap it */
      animation: fadeInBox 1.3s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
      display: flex;
      flex-direction: column;
      align-items: center;
      opacity: 0; /* Start hidden to fade in after spinner */
      transform: scale(0.94) translateY(10px); /* Initial state for animation */
    }
    /* Keyframes for main box fade-in, triggered by JS after spinner hides */
    @keyframes fadeInBox {
      0% { opacity: 0; transform: scale(0.94) translateY(10px);}
      100% { opacity: 1; transform: scale(1) translateY(0);}
    }

    /* Added pulsing glow animation for text */
    @keyframes pulseGlow {
      0% { text-shadow: 0 2px 12px #8b0000aa; }
      50% { text-shadow: 0 2px 20px #8b0000dd, 0 0 30px #ff4d4daa; }
      100% { text-shadow: 0 2px 12px #8b0000aa; }
    }
    .glow-red {
      animation: pulseGlow 2.5s infinite ease-in-out;
      animation-delay: 1.5s; /* Start after initial page animations */
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
      margin-bottom: 20px; /* Increased margin */
      direction: rtl;
      font-family: 'Cairo', 'Segoe UI', 'Arial', 'Noto Naskh Arabic', serif;
      font-weight: 600;
    }
    .socials {
      display: flex;
      justify-content: center;
      gap: 20px; /* Increased gap for bigger icons */
      margin: 12px 0 10px 0; /* Adjusted margin */
      flex-wrap: wrap;
    }

    /* Keyframes for icon pop-in animation */
    @keyframes iconPopIn {
      0% {
        opacity: 0;
        transform: scale(0.3) translateY(20px);
      }
      60% {
        opacity: 1;
        transform: scale(1.1) translateY(-5px); /* Overshoot */
      }
      100% {
        opacity: 1;
        transform: scale(1) translateY(0);
      }
    }

    .socials a {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 56px; /* Increased icon container size */
      height: 56px; /* Increased icon container size */
      border-radius: 50%;
      background: #fff;
      box-shadow: 0 3px 15px #1976d233; /* Slightly enhanced base shadow */
      transition: transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1), box-shadow 0.3s cubic-bezier(0.34, 1.56, 0.64, 1), border-color 0.3s ease-out; /* Smoother, bouncier transition */
      border: 2.5px solid #b3e0ff; /* Slightly thicker border */
      position: relative;
      overflow: hidden;

      /* Apply pop-in animation */
      opacity: 0; /* Start hidden for animation */
      transform: scale(0.3); /* Initial state for animation */
      animation-name: iconPopIn;
      animation-duration: 0.6s;
      animation-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55); /* Bouncy effect */
      animation-fill-mode: forwards;
    }

    /* Staggered animation delays for icons - starting after main box fades in */
    .socials a:nth-child(1) { animation-delay: 1.3s; }
    .socials a:nth-child(2) { animation-delay: 1.4s; }
    .socials a:nth-child(3) { animation-delay: 1.5s; }
    .socials a:nth-child(4) { animation-delay: 1.6s; }


    .socials a:hover {
      transform: scale(1.20) rotate(-8deg); /* Enhanced hover: larger scale, more rotation */
      box-shadow: 0 8px 25px #1976d288; /* More pronounced shadow on hover */
      border-color: #1976d2b3; /* Darker border on hover */
    }
    .social-icon {
      width: 30px; /* Increased SVG icon size */
      height: 30px; /* Increased SVG icon size */
      display: block;
      transition: transform 0.25s ease-out; /* Transition for icon scaling */
    }
    .socials a:hover .social-icon {
      transform: scale(1.1); /* Scale the SVG itself on hover */
    }

    .footer {
      color: #1976d2;
      background: rgba(25, 118, 210, 0.07);
      border-radius: 8px;
      margin: 28px auto 0 auto; /* Increased top margin */
      max-width: 340px;
      padding: 10px 15px;
      font-size: 0.97em;
      animation: fadeIn 2s 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards; /* Delayed footer fade-in */
      opacity: 0;
      font-family: 'Inter', 'Cairo', 'Segoe UI', Arial, sans-serif;
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(5px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    /* Loading Spinner Styles */
    #loading-spinner {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: #b3e0ff; /* Match body background */
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 1000;
      transition: opacity 0.5s ease-out;
    }

    .spinner {
      border: 8px solid #f3f3f3; /* Light grey */
      border-top: 8px solid #1976d2; /* Blue */
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: spin 1.2s linear infinite;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    /* Copied Message Styles */
    .copied-message {
      position: absolute;
      background-color: #4CAF50; /* Green background */
      color: white;
      padding: 5px 10px;
      border-radius: 5px;
      font-size: 0.8em;
      opacity: 0;
      transition: opacity 0.5s ease-out, transform 0.5s ease-out;
      pointer-events: none; /* Allow clicks to pass through */
      white-space: nowrap;
      z-index: 10; /* Ensure it's above other elements */
    }

    .copied-message.show {
      opacity: 1;
      transform: translateY(-20px); /* Move up slightly */
    }

    /* Responsive Design */
    @media (max-width: 540px) {
      body {
        padding: 15px 0;
        height: auto;
        min-height: 100vh;
        align-items: flex-start;
      }
      .main-box {
        margin: 20px auto; /* Centered on mobile */
        padding: 25px 5vw 20px 5vw; /* Adjusted padding for vw */
        max-width: 95vw;
        border-radius: 12px;
      }
      .title-line1 {
        font-size: 1.7em; /* Adjusted for new icon sizes */
      }
      .title-line2 {
        font-size: 0.95em; /* Adjusted */
      }
       .follow-us {
        font-size: 1.0em;
        margin-bottom: 15px;
      }
      .footer {
        max-width: 90vw;
        font-size: 0.88em; /* Adjusted */
        padding: 8px 10px;
      }
      .socials {
        gap: 15px; /* Adjusted gap for mobile */
      }
      .socials a {
        width: 48px; /* Adjusted icon size for mobile */
        height: 48px; /* Adjusted icon size for mobile */
      }
      .social-icon {
        width: 26px; /* Adjusted SVG size for mobile */
        height: 26px; /* Adjusted SVG size for mobile */
      }
    }
  </style>
</head>
<body>
  <div id="loading-spinner">
    <div class="spinner"></div>
  </div>

  <div class="main-box" id="main-content">
    <div class="main-title glow-red">
      <div class="title-line1">فريق ابناء كوش</div>
      <div class="title-line2">للعبادة و التسبيح</div>
    </div>
    <div class="follow-us glow-red">تابعونا على منصات التواصل الاجتماعي</div>
    <div class="socials">
      <a href="https://www.instagram.com/abnaa.kush/" target="_blank" title="Instagram" aria-label="Instagram">
        <svg class="social-icon" viewBox="0 0 50 50">
          <defs>
            <radialGradient id="ig" cx="0.35" cy="0.95" r="1.5"> <stop offset="0%" stop-color="#fdf497"/>
              <stop offset="25%" stop-color="#fd5949"/>
              <stop offset="50%" stop-color="#d6249f"/>
              <stop offset="100%" stop-color="#285AEB"/>
            </radialGradient>
          </defs>
          <path d="M25 4.5 A 20.5 20.5 0 1 0 25 45.5 A 20.5 20.5 0 1 0 25 4.5 Z" fill="url(#ig)"/>
          <path d="M25 12.5 A 12.5 12.5 0 1 0 25 37.5 A 12.5 12.5 0 1 0 25 12.5 Z" fill="none" stroke="#fff" stroke-width="2.5"/>
          <path d="M25 17.5 A 7.5 7.5 0 1 0 25 32.5 A 7.5 7.5 0 1 0 25 17.5 Z" fill="none" stroke="#fff" stroke-width="2.5"/>
          <circle cx="34" cy="16" r="2.5" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.facebook.com/profile.php?id=61561245110328" target="_blank" title="Facebook" aria-label="Facebook">
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#1877F3"/>
          <path d="M29 38V26h4l1-6h-5v-3c0-1.7.6-3 2.4-3H34V9.5C33.4 9.4 32 9 30.3 9 26.4 9 24 11.1 24 15v5h-4v6h4v12h6z" fill="#fff"/>
        </svg>
      </a>
      <a href="https://www.tiktok.com/@abnaakush8" target="_blank" title="TikTok" aria-label="TikTok">
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#000"/>
          <path d="M32.5 18.5c1.7 0 3.2-.7 4.3-1.7v4.3c-1.3.1-2.6-.1-3.8-.5v8.7c0 4.6-3.7 8.3-8.3 8.3s-8.3-3.7-8.3-8.3 3.7-8.3 8.3-8.3v4.1c-2.3 0-4.2 1.9-4.2 4.2 0 2.3 1.9 4.2 4.2 4.2 2.3 0 4.2-1.9 4.2-4.2V13.2c1.1.7 2.4 1.3 3.8 1.3z" fill="#fff"/>
          <path d="M36.8 16.8c-1.1 1-2.7 1.7-4.3 1.7-1.4 0-2.7-.6-3.8-1.3v2c1.2.4 2.5.6 3.8.5v-2.9c1.1.7 2.4 1.3 3.8 1.3v-1.3h.5z" fill="#25F4EE"/>
          <path d="M28.7 11.5v17.8c0 2.3-1.9 4.2-4.2 4.2s-4.2-1.9-4.2-4.2c0-2.3 1.9-4.2 4.2-4.2v-2c-4.6 0-8.3 3.7-8.3 8.3s3.7 8.3 8.3 8.3 8.3-3.7 8.3-8.3V12.8c-1.4-.3-2.7-.8-3.8-1.3z" fill="#FE2C55"/>
        </svg>
      </a>
      <a href="https://www.youtube.com/@abnaakush" target="_blank" title="YouTube" aria-label="YouTube">
        <svg class="social-icon" viewBox="0 0 50 50">
          <circle cx="25" cy="25" r="22" fill="#FF0000"/>
          <polygon points="20,17 37,25 20,33" fill="#fff"/>
        </svg>
      </a>
    </div>
    <div class="footer">
      © 2025 فريق ابناء كوش للعبادة و التسبيح. جميع الحقوق محفوظة.
    </div>
  </div>

  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const loadingSpinner = document.getElementById('loading-spinner');
      const mainContent = document.getElementById('main-content');
      const socialLinks = document.querySelectorAll('.socials a');

      // Show spinner initially
      loadingSpinner.style.opacity = '1';
      loadingSpinner.style.display = 'flex';

      // Hide spinner and show main content after a delay
      setTimeout(() => {
        loadingSpinner.style.opacity = '0';
        // Use a small delay before hiding display to allow transition to complete
        setTimeout(() => {
          loadingSpinner.style.display = 'none';
          mainContent.style.opacity = '1'; // Fade in main content
          mainContent.style.transform = 'scale(1) translateY(0)'; // Apply final transform
        }, 500); // Matches opacity transition duration
      }, 2000); // Spinner visible for 2 seconds

      // Function to show "Copied!" message
      function showCopiedMessage(element) {
        // Remove any existing message for this element
        let existingMessage = element.querySelector('.copied-message');
        if (existingMessage) {
          existingMessage.remove();
        }

        const message = document.createElement('span');
        message.className = 'copied-message';
        message.textContent = 'Copied!';
        element.appendChild(message);

        // Position the message relative to the icon
        const iconRect = element.getBoundingClientRect();
        message.style.left = `${(iconRect.width / 2) - (message.offsetWidth / 2)}px`; // Center horizontally
        message.style.top = `-${iconRect.height / 2}px`; // Position above the icon

        // Trigger fade-in and slide-up animation
        setTimeout(() => {
          message.classList.add('show');
        }, 10); // Small delay to allow reflow before animation

        // Hide and remove message after a delay
        setTimeout(() => {
          message.classList.remove('show');
          setTimeout(() => {
            message.remove();
          }, 500); // Matches transition duration
        }, 1500); // Message visible for 1.5 seconds
      }

      // Add click event listeners to social links
      socialLinks.forEach(link => {
        link.addEventListener('click', (event) => {
          event.preventDefault(); // Prevent default link behavior (opening new tab immediately)

          const urlToCopy = link.href;

          // Copy URL to clipboard
          const tempInput = document.createElement('textarea');
          tempInput.value = urlToCopy;
          document.body.appendChild(tempInput);
          tempInput.select();
          try {
            document.execCommand('copy');
            showCopiedMessage(link); // Show "Copied!" message on success
          } catch (err) {
            console.error('Failed to copy text: ', err);
            // Optionally, show an error message to the user
          } finally {
            document.body.removeChild(tempInput);
          }

          // Open the link in a new tab after a short delay to allow message to show
          setTimeout(() => {
            window.open(urlToCopy, '_blank');
          }, 500); // Adjust delay as needed
        });
      });
    });
  </script>
</body>
</html>
![Uploading image.png…]()
