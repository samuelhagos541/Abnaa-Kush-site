<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فريق أبناء كوش للعبادة والتسبيح | Sons of Kush</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;700&family=Tajawal:wght@300;400;700&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Tajawal', 'Outfit', 'sans-serif'],
                    },
                    colors: {
                        primary: '#1e3a8a', // Deep Blue
                        secondary: '#eab308', // Gold/Yellow
                        accent: '#f8fafc',
                    }
                }
            }
        }
    </script>
    <style>
        /* Smooth transitions for language switching */
        body {
            transition: background-color 0.3s, color 0.3s;
        }
        .fade-in {
            animation: fadeIn 0.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Make sure videos maintain a 16:9 aspect ratio */
        .aspect-w-16 { position: relative; padding-bottom: 56.25%; }
        .aspect-w-16 > * { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-secondary selection:text-primary">

    <!-- Navigation -->
    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
                
                <!-- Logo / Title -->
                <div class="flex-shrink-0 flex items-center gap-3 cursor-pointer">
                    <div class="w-10 h-10 bg-primary text-secondary rounded-full flex items-center justify-center text-xl shadow-lg">
                        <i class="fa-solid fa-music"></i>
                    </div>
                    <span class="font-bold text-xl md:text-2xl text-primary" data-i18n="nav_title">أبناء كوش</span>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center gap-8">
                    <a href="#home" class="text-slate-600 hover:text-primary font-semibold transition-colors" data-i18n="nav_home">الرئيسية</a>
                    <a href="#videos" class="text-slate-600 hover:text-primary font-semibold transition-colors" data-i18n="nav_videos">فيديوهاتنا</a>
                    <a href="#social" class="text-slate-600 hover:text-primary font-semibold transition-colors" data-i18n="nav_social">التواصل</a>
                    
                    <!-- Language Toggle -->
                    <button onclick="toggleLanguage()" class="flex items-center gap-2 bg-slate-100 hover:bg-slate-200 text-slate-700 px-4 py-2 rounded-full transition-colors border border-slate-200">
                        <i class="fa-solid fa-globe"></i>
                        <span id="lang-btn-text">English</span>
                    </button>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center gap-4">
                    <button onclick="toggleLanguage()" class="text-slate-600 hover:text-primary">
                        <i class="fa-solid fa-globe text-xl"></i>
                    </button>
                    <button class="text-slate-600 hover:text-primary focus:outline-none" id="mobile-menu-btn">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile Menu Dropdown -->
        <div class="md:hidden hidden bg-white border-t border-slate-100" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:text-primary hover:bg-slate-50" data-i18n="nav_home">الرئيسية</a>
                <a href="#videos" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:text-primary hover:bg-slate-50" data-i18n="nav_videos">فيديوهاتنا</a>
                <a href="#social" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:text-primary hover:bg-slate-50" data-i18n="nav_social">التواصل</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="home" class="relative bg-primary text-white overflow-hidden">
        <!-- Abstract Background shapes -->
        <div class="absolute inset-0 opacity-10">
            <svg class="absolute -top-24 -end-24 w-96 h-96 text-white" fill="currentColor" viewBox="0 0 100 100"><circle cx="50" cy="50" r="50"/></svg>
            <svg class="absolute top-1/2 -start-24 w-64 h-64 text-secondary" fill="currentColor" viewBox="0 0 100 100"><circle cx="50" cy="50" r="50"/></svg>
        </div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 py-24 md:py-32 flex flex-col items-center text-center fade-in">
            <span class="bg-white/20 text-secondary border border-white/30 px-4 py-1 rounded-full text-sm font-semibold tracking-wide mb-6 backdrop-blur-sm" data-i18n="hero_badge">مرحباً بكم | Welcome</span>
            <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight" data-i18n="hero_title">
                فريق أبناء كوش للعبادة والتسبيح
            </h1>
            <p class="text-lg md:text-2xl text-blue-100 max-w-2xl mb-10" data-i18n="hero_subtitle">
                نرفع أصواتنا في العبادة والتسبيح لتمجيد اسمه. تابع أحدث أعمالنا وترانيمنا هنا.
            </p>
            <div class="flex flex-col sm:flex-row gap-4">
                <a href="#videos" class="bg-secondary hover:bg-yellow-400 text-primary font-bold text-lg px-8 py-3 rounded-full shadow-lg transition-transform transform hover:scale-105" data-i18n="btn_watch">شاهد الفيديوهات</a>
                <a href="#social" class="bg-transparent border-2 border-white/50 hover:bg-white/10 text-white font-bold text-lg px-8 py-3 rounded-full transition-colors" data-i18n="btn_contact">تواصل معنا</a>
            </div>
        </div>
    </header>

    <!-- Videos Section -->
    <section id="videos" class="py-20 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl md:text-4xl font-bold text-primary mb-4" data-i18n="section_videos_title">أحدث الفيديوهات</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
                <p class="mt-4 text-slate-500 max-w-2xl mx-auto" data-i18n="section_videos_desc">مجموعة من أحدث الترانيم والتسبيحات من قناتنا على يوتيوب.</p>
            </div>

            <!-- Videos Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Placeholder Video 1 -->
                <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition-shadow group">
                    <div class="aspect-w-16 bg-black relative flex items-center justify-center">
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/w00bzpbGVZs?rel=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-800 mb-2" data-i18n="video_1_title">ترنيمة يا سامع الصلاة</h3>
                        <p class="text-sm text-slate-500" data-i18n="video_1_date">تم النشر: ٢١ نوفمبر ٢٠١٩</p>
                    </div>
                </div>

                <!-- Video 2 -->
                <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition-shadow group">
                    <div class="aspect-w-16 bg-black relative flex items-center justify-center">
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/le_EB1W5v0Q?rel=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-800 mb-2" data-i18n="video_2_title">انت سيد الكون</h3>
                        <p class="text-sm text-slate-500" data-i18n="video_2_date">تم النشر: ٣١ مارس ٢٠٢٥</p>
                    </div>
                </div>

                <!-- Video 3 -->
                <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition-shadow group">
                    <div class="aspect-w-16 bg-black relative flex items-center justify-center">
                        <iframe class="absolute top-0 left-0 w-full h-full" src="https://www.youtube.com/embed/DQMGlNxsbrE?rel=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-800 mb-2" data-i18n="video_3_title">ترنيمة : داير اعبدك</h3>
                        <p class="text-sm text-slate-500" data-i18n="video_3_date">تم النشر: ١١ أكتوبر ٢٠٢٢</p>
                    </div>
                </div>

            </div>
            
            <div class="text-center mt-12">
                <a href="https://www.youtube.com/@abnaakush4081" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 text-primary font-bold hover:text-secondary transition-colors text-lg group">
                    <span data-i18n="btn_more_videos">شاهد المزيد على قناتنا</span>
                    <i class="fa-solid fa-arrow-right rtl:rotate-180 transform group-hover:translate-x-1 rtl:group-hover:-translate-x-1 transition-transform"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Social Media Videos Section -->
    <section id="social-videos" class="py-20 bg-slate-200 border-t border-slate-300 shadow-inner">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl md:text-4xl font-bold text-primary mb-4" data-i18n="section_social_videos_title">فيديوهات مميزة من منصاتنا</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
                <p class="mt-4 text-slate-600 max-w-2xl mx-auto" data-i18n="section_social_videos_desc">أشهر المقاطع والترانيم القصيرة من حساباتنا على تيك توك وفيسبوك.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-10 max-w-4xl mx-auto">
                <!-- Facebook Video Embed -->
                <div class="bg-white rounded-2xl shadow-lg overflow-hidden hover:shadow-xl transition-shadow border-t-4 border-blue-600 flex flex-col">
                    <div class="p-4 bg-blue-50 flex items-center justify-between">
                        <div class="flex items-center gap-3">
                            <i class="fa-brands fa-facebook text-2xl text-blue-600"></i>
                            <h3 class="font-bold text-slate-800" data-i18n="fb_video_title">ريلز فيسبوك | Facebook Reel</h3>
                        </div>
                    </div>
                    <!-- Embed Container -->
                    <div class="bg-slate-100 flex justify-center items-center overflow-hidden w-full" style="min-height: 500px;">
                         <iframe src="https://www.facebook.com/plugins/video.php?height=720&href=https%3A%2F%2Fwww.facebook.com%2Freel%2F1BTAffYwRx&show_text=false&width=405&t=0" width="405" height="720" style="border:none;overflow:hidden; max-width: 100%;" scrolling="no" frameborder="0" allowfullscreen allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
                    </div>
                </div>

                <!-- TikTok Video Placeholder -->
                <div class="bg-white rounded-2xl shadow-lg overflow-hidden hover:shadow-xl transition-shadow border-t-4 border-black flex flex-col">
                    <div class="p-4 bg-slate-50 flex items-center justify-between">
                        <div class="flex items-center gap-3">
                            <i class="fa-brands fa-tiktok text-2xl text-black"></i>
                            <h3 class="font-bold text-slate-800" data-i18n="tiktok_video_title">الأكثر مشاهدة على تيك توك</h3>
                        </div>
                    </div>
                    <!-- TikTok Embed -->
                    <div class="bg-slate-100 flex justify-center items-center overflow-hidden w-full h-full" style="min-height: 500px;">
                        <blockquote class="tiktok-embed" cite="https://www.tiktok.com/@abnaakush8/video/7584555148798708999" data-video-id="7584555148798708999" style="max-width: 605px;min-width: 325px;" > <section> <a target="_blank" title="@abnaakush8" href="https://www.tiktok.com/@abnaakush8?refer=embed">@abnaakush8</a> بمسيحنا الغالي نفخر لا بنداري ولا بنخجل🙏🏾🙏🏾❤️ <a title="ترانيم_سودانية" target="_blank" href="https://www.tiktok.com/tag/%D8%AA%D8%B1%D8%A7%D9%86%D9%8A%D9%85_%D8%B3%D9%88%D8%AF%D8%A7%D9%86%D9%8A%D8%A9?refer=embed">#ترانيم_سودانية</a> <a title="ابناء_كوش" target="_blank" href="https://www.tiktok.com/tag/%D8%A7%D8%A8%D9%86%D8%A7%D8%A1_%D9%83%D9%88%D8%B4?refer=embed">#ابناء_كوش</a> <a title="السودان" target="_blank" href="https://www.tiktok.com/tag/%D8%A7%D9%84%D8%B3%D9%88%D8%AF%D8%A7%D9%86?refer=embed">#السودان</a> <a target="_blank" title="♬ original sound  - AbnaaKush" href="https://www.tiktok.com/music/original-sound-AbnaaKush-7584555224770136840?refer=embed">♬ original sound  - AbnaaKush</a> </section> </blockquote> <script async src="https://www.tiktok.com/embed.js"></script>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Media Section -->
    <section id="social" class="py-20 bg-white border-t border-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center fade-in">
            <h2 class="text-3xl md:text-4xl font-bold text-primary mb-4" data-i18n="section_social_title">تابعونا على المنصات</h2>
            <div class="w-24 h-1 bg-secondary mx-auto rounded-full mb-12"></div>
            
            <div class="flex flex-wrap justify-center gap-6 md:gap-10">
                <!-- Facebook -->
                <a href="https://www.facebook.com/profile.php?id=61561245110328&sk=about" target="_blank" rel="noopener noreferrer" class="w-20 h-20 md:w-24 md:h-24 bg-blue-50 text-blue-600 rounded-full flex flex-col items-center justify-center hover:bg-blue-600 hover:text-white transition-all transform hover:-translate-y-2 shadow-sm hover:shadow-lg">
                    <i class="fa-brands fa-facebook-f text-3xl md:text-4xl mb-1"></i>
                </a>
                <!-- YouTube -->
                <a href="https://www.youtube.com/@abnaakush4081" target="_blank" rel="noopener noreferrer" class="w-20 h-20 md:w-24 md:h-24 bg-red-50 text-red-600 rounded-full flex flex-col items-center justify-center hover:bg-red-600 hover:text-white transition-all transform hover:-translate-y-2 shadow-sm hover:shadow-lg">
                    <i class="fa-brands fa-youtube text-3xl md:text-4xl mb-1"></i>
                </a>
                <!-- Instagram -->
                <a href="https://www.instagram.com/abnaa.kush" target="_blank" rel="noopener noreferrer" class="w-20 h-20 md:w-24 md:h-24 bg-pink-50 text-pink-600 rounded-full flex flex-col items-center justify-center hover:bg-gradient-to-tr hover:from-yellow-400 hover:via-pink-500 hover:to-purple-600 hover:text-white transition-all transform hover:-translate-y-2 shadow-sm hover:shadow-lg">
                    <i class="fa-brands fa-instagram text-3xl md:text-4xl mb-1"></i>
                </a>
                <!-- TikTok -->
                <a href="https://www.tiktok.com/@abnaakush8" target="_blank" rel="noopener noreferrer" class="w-20 h-20 md:w-24 md:h-24 bg-slate-100 text-slate-800 rounded-full flex flex-col items-center justify-center hover:bg-black hover:text-white transition-all transform hover:-translate-y-2 shadow-sm hover:shadow-lg">
                    <i class="fa-brands fa-tiktok text-3xl md:text-4xl mb-1"></i>
                </a>
                <!-- Email -->
                <a href="mailto:abnaakushworshipteam@gmail.com" class="w-20 h-20 md:w-24 md:h-24 bg-teal-50 text-teal-600 rounded-full flex flex-col items-center justify-center hover:bg-teal-600 hover:text-white transition-all transform hover:-translate-y-2 shadow-sm hover:shadow-lg">
                    <i class="fa-solid fa-envelope text-3xl md:text-4xl mb-1"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-primary text-slate-300 py-10 border-t border-primary/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between gap-6">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 bg-primary border-2 border-secondary text-secondary rounded-full flex items-center justify-center text-xl shadow-lg">
                    <i class="fa-solid fa-music text-lg"></i>
                </div>
                <span class="font-bold text-white text-lg" data-i18n="nav_title">أبناء كوش</span>
            </div>
            
            <p class="text-sm text-center md:text-start" data-i18n="footer_copyright">
                &copy; 2026 فريق أبناء كوش للعبادة والتسبيح. جميع الحقوق محفوظة.
            </p>
        </div>
    </footer>

    <!-- Translations & Interactivity Script -->
    <script>
        // Translations Dictionary
        const translations = {
            ar: {
                nav_title: "أبناء كوش",
                nav_home: "الرئيسية",
                nav_videos: "فيديوهاتنا",
                nav_social: "التواصل",
                hero_badge: "مرحباً بكم",
                hero_title: "فريق أبناء كوش للعبادة والتسبيح",
                hero_subtitle: "نرفع أصواتنا في العبادة والتسبيح لتمجيد اسمه. تابع أحدث أعمالنا وترانيمنا هنا.",
                btn_watch: "شاهد الفيديوهات",
                btn_contact: "تواصل معنا",
                section_videos_title: "أحدث الفيديوهات",
                section_videos_desc: "مجموعة من أحدث الترانيم والتسبيحات من قناتنا على يوتيوب.",
                video_1_title: "ترنيمة يا سامع الصلاة - فريق أبناء كوش (كلمات وألحان: جورج جون)",
                video_1_date: "تم النشر: ٢١ نوفمبر ٢٠١٩",
                video_2_title: "انت سيد الكون - كلمات يعقوب عزرا",
                video_2_date: "تم النشر: ٣١ مارس ٢٠٢٥",
                video_3_title: "ترنيمة : داير اعبدك - فريق أبناء كوش للعبادة و التسبيح",
                video_3_date: "تم النشر: ١١ أكتوبر ٢٠٢٢",
                btn_more_videos: "شاهد المزيد على قناتنا",
                section_social_videos_title: "فيديوهات مميزة من منصاتنا",
                section_social_videos_desc: "أشهر المقاطع والترانيم القصيرة من حساباتنا على تيك توك وفيسبوك.",
                fb_video_title: "ترنيمة نعم المسيح",
                tiktok_video_title: "بمسيحنا الغالي نفخر",
                placeholder_link_needed: "يرجى توفير رابط الفيديو المباشر لإضافته هنا",
                section_social_title: "تابعونا على المنصات",
                footer_copyright: "© 2026 فريق أبناء كوش للعبادة والتسبيح. جميع الحقوق محفوظة."
            },
            en: {
                nav_title: "Sons of Kush",
                nav_home: "Home",
                nav_videos: "Videos",
                nav_social: "Contact",
                hero_badge: "Welcome",
                hero_title: "Sons of Kush Worship & Praise Team",
                hero_subtitle: "Lifting our voices in worship and praise to glorify His name. Follow our latest hymns here.",
                btn_watch: "Watch Videos",
                btn_contact: "Contact Us",
                section_videos_title: "Latest Videos",
                section_videos_desc: "A collection of the latest hymns and praises from our YouTube channel.",
                video_1_title: "Hymn: O Hearer of Prayer - Sons of Kush (Words & Melody: George John)",
                video_1_date: "Published: Nov 21, 2019",
                video_2_title: "You Are the Lord of the Universe - Words by Yacoub Ezra",
                video_2_date: "Published: Mar 31, 2025",
                video_3_title: "Hymn: Dayr Aabudak - Sons of Kush Worship and Praise Team",
                video_3_date: "Published: Oct 11, 2022",
                btn_more_videos: "Watch more on our channel",
                section_social_videos_title: "Featured Social Videos",
                section_social_videos_desc: "The most popular short clips and hymns from our TikTok and Facebook.",
                fb_video_title: "Hymn: Naam Al Maseeh",
                tiktok_video_title: "We Boast in Our Precious Christ",
                placeholder_link_needed: "Please provide the direct video link to embed it here",
                section_social_title: "Follow Us Online",
                footer_copyright: "© 2026 Sons of Kush Worship and Praise Team. All rights reserved."
            }
        };

        let currentLang = 'ar';

        function toggleLanguage() {
            // Swap language
            currentLang = currentLang === 'ar' ? 'en' : 'ar';
            const isAr = currentLang === 'ar';
            
            // Update HTML attributes for layout flow
            document.documentElement.lang = currentLang;
            document.documentElement.dir = isAr ? 'rtl' : 'ltr';

            // Update button text
            document.getElementById('lang-btn-text').innerText = isAr ? 'English' : 'عربي';

            // Translate all elements with data-i18n attribute
            const elementsToTranslate = document.querySelectorAll('[data-i18n]');
            elementsToTranslate.forEach(el => {
                const key = el.getAttribute('data-i18n');
                if (translations[currentLang][key]) {
                    el.innerText = translations[currentLang][key];
                }
            });
        }

        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu on link click
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
