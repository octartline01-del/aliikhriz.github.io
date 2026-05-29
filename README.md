# aliikhriz.github.io[index.html](https://github.com/user-attachments/files/28406075/index.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhamad Ali Khoirul Rizal - Professional Hospitality Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Cinzel & Plus Jakarta Sans -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        cinzel: ['Cinzel', 'serif'],
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                    },
                    colors: {
                        navy: {
                            950: '#01040f',
                            900: '#020617',
                            800: '#07122c',
                            700: '#0e1e43',
                            600: '#1b2e5c',
                        },
                        gold: {
                            100: '#fcf8ec',
                            200: '#f5e6c4',
                            300: '#e5ca89',
                            400: '#d4af37',
                            500: '#aa841a',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom Premium Glassmorphism */
        .glass-panel {
            background: rgba(7, 18, 44, 0.45);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(212, 175, 55, 0.15);
        }
        
        .glass-card {
            background: rgba(14, 30, 67, 0.35);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(212, 175, 55, 0.1);
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .glass-card:hover {
            background: rgba(14, 30, 67, 0.6);
            border-color: rgba(212, 175, 55, 0.35);
            transform: translateY(-4px);
            box-shadow: 0 10px 30px -10px rgba(212, 175, 55, 0.15);
        }

        /* Gold Gradient Text */
        .text-gold-gradient {
            background: linear-gradient(135deg, #f5e6c4 0%, #d4af37 50%, #aa841a 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Ambient Glow Animations */
        @keyframes rotateRing {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            100% { transform: translate(-50%, -50%) rotate(360deg); }
        }

        @keyframes pulseGlow {
            0%, 100% { opacity: 0.2; transform: scale(1); }
            50% { opacity: 0.4; transform: scale(1.05); }
        }

        .ambient-glow {
            animation: pulseGlow 8s ease-in-out infinite;
        }

        .rotating-gold-border {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 104%;
            height: 104%;
            border: 2px dashed rgba(212, 175, 55, 0.4);
            border-radius: 50%;
            animation: rotateRing 25s linear infinite;
        }

        /* Scrollbar styling */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #020617;
        }
        ::-webkit-scrollbar-thumb {
            background: rgba(212, 175, 55, 0.3);
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: rgba(212, 175, 55, 0.5);
        }

        /* Smooth Anchor Scroll */
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-navy-900 text-slate-100 font-sans selection:bg-gold-400 selection:text-navy-900 overflow-x-hidden">

    <!-- Ambient Backdrops (Futuristic Glows) -->
    <div class="absolute top-0 left-1/4 w-[500px] h-[500px] bg-gold-400/5 rounded-full filter blur-[120px] pointer-events-none ambient-glow"></div>
    <div class="absolute top-[800px] right-1/4 w-[600px] h-[600px] bg-navy-600/10 rounded-full filter blur-[150px] pointer-events-none ambient-glow" style="animation-delay: -3s;"></div>
    <div class="absolute bottom-10 left-1/3 w-[450px] h-[450px] bg-gold-400/5 rounded-full filter blur-[110px] pointer-events-none ambient-glow" style="animation-delay: -5s;"></div>

    <!-- Navigation Header -->
    <header class="fixed top-0 left-0 w-full z-50 transition-all duration-300" id="mainHeader">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-10 h-10 rounded-lg flex items-center justify-center bg-gradient-to-br from-gold-300 to-gold-500 p-[1px]">
                    <div class="w-full h-full bg-navy-800 rounded-[7px] flex items-center justify-center transition-colors group-hover:bg-navy-700">
                        <i data-lucide="hotel" class="w-5 h-5 text-gold-300"></i>
                    </div>
                </div>
                <div class="flex flex-col">
                    <span class="font-cinzel text-md font-bold tracking-widest text-gold-300 group-hover:text-gold-200 transition-colors">A. RIZAL</span>
                    <span class="text-[9px] uppercase tracking-[0.25em] text-slate-400">Hospitality</span>
                </div>
            </a>

            <!-- Action Navigation Links (Large Screens) -->
            <div class="hidden md:flex items-center gap-8">
                <a href="#about" class="text-xs uppercase tracking-widest text-slate-300 hover:text-gold-300 transition-colors">Profil</a>
                <a href="#skills" class="text-xs uppercase tracking-widest text-slate-300 hover:text-gold-300 transition-colors">Keahlian</a>
                <a href="#experience" class="text-xs uppercase tracking-widest text-slate-300 hover:text-gold-300 transition-colors">Pengalaman</a>
                <a href="#ai-interviewer" class="text-xs uppercase tracking-widest text-gold-300 hover:text-gold-200 transition-colors flex items-center gap-1.5 font-semibold">
                    <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> AI Assistant
                </a>
            </div>

            <!-- Action Menu Trigger (Garis 3 / Hamburger) -->
            <button id="menuBtn" class="relative z-50 p-3 flex flex-col justify-center items-center w-12 h-12 rounded-full glass-panel hover:border-gold-400/50 group transition-all duration-300" aria-label="Menu">
                <span id="line1" class="w-5 h-[2px] bg-gold-300 rounded-full transition-all duration-300 translate-y-[-4px] group-hover:bg-gold-200"></span>
                <span id="line2" class="w-5 h-[2px] bg-gold-300 rounded-full transition-all duration-300 group-hover:bg-gold-200"></span>
                <span id="line3" class="w-5 h-[2px] bg-gold-300 rounded-full transition-all duration-300 translate-y-[4px] group-hover:bg-gold-200"></span>
            </button>
        </div>
    </header>

    <!-- Side Navigation Menu (Drawer Overlay) -->
    <div id="sideMenu" class="fixed inset-0 z-40 bg-navy-900/80 backdrop-blur-md opacity-0 pointer-events-none transition-all duration-500 flex justify-end">
        <div class="w-full max-w-md h-full bg-navy-800/90 border-l border-gold-400/10 p-12 flex flex-col justify-between transform translate-x-full transition-transform duration-500 ease-out shadow-2xl relative" id="drawerContent">
            
            <!-- Top brand inside menu -->
            <div class="flex items-center gap-3">
                <i data-lucide="hotel" class="w-6 h-6 text-gold-300"></i>
                <span class="font-cinzel text-lg font-bold tracking-widest text-gold-300">MENU</span>
            </div>

            <!-- Central Links -->
            <div class="space-y-8 my-auto">
                <a href="#" class="block text-3xl font-cinzel text-slate-300 hover:text-gold-300 transition-colors duration-300" onclick="toggleMenu()">BERANDA</a>
                <a href="#about" class="block text-3xl font-cinzel text-slate-300 hover:text-gold-300 transition-colors duration-300" onclick="toggleMenu()">PROFIL SAYA</a>
                <a href="#skills" class="block text-3xl font-cinzel text-slate-300 hover:text-gold-300 transition-colors duration-300" onclick="toggleMenu()">KEAHLIAN</a>
                <a href="#experience" class="block text-3xl font-cinzel text-slate-300 hover:text-gold-300 transition-colors duration-300" onclick="toggleMenu()">PENGALAMAN</a>
                <a href="#ai-interviewer" class="block text-3xl font-cinzel text-gold-300 hover:text-gold-200 transition-colors duration-300 flex items-center gap-2" onclick="toggleMenu()">
                    <i data-lucide="sparkles" class="w-6 h-6 text-gold-300"></i> AI ASSISTANT
                </a>
                <hr class="border-gold-400/10">
                <!-- Contact Us Trigger -->
                <a href="https://wa.me/6283159970756" target="_blank" rel="noopener noreferrer" class="group flex items-center justify-between p-4 rounded-xl bg-gradient-to-r from-gold-500/10 to-gold-300/5 border border-gold-400/20 hover:border-gold-400 transition-all duration-300">
                    <div class="flex items-center gap-3">
                        <i data-lucide="message-square-text" class="w-5 h-5 text-gold-300 group-hover:scale-110 transition-transform"></i>
                        <div>
                            <p class="font-semibold text-gold-300 text-sm">CONTACT US</p>
                            <p class="text-[10px] text-slate-400">Hubungi langsung via WhatsApp</p>
                        </div>
                    </div>
                    <i data-lucide="arrow-right" class="w-5 h-5 text-gold-300 group-hover:translate-x-1 transition-transform"></i>
                </a>
            </div>

            <!-- Footer info in drawer -->
            <div class="text-xs text-slate-500">
                <p>&copy; 2026 Muhamad Ali Khoirul Rizal.</p>
                <p class="mt-1">SMKN 9 Bandung - Perhotelan</p>
            </div>
        </div>
    </div>

    <!-- Hero Section -->
    <section class="min-h-screen flex items-center pt-28 pb-16 px-6 relative z-10">
        <div class="max-w-7xl mx-auto w-full grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            
            <!-- LEFT: Profile Text Content -->
            <div class="lg:col-span-7 flex flex-col justify-center space-y-6 text-center lg:text-left order-2 lg:order-1">
                <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-gold-400/10 border border-gold-400/20 w-fit mx-auto lg:mx-0">
                    <span class="w-1.5 h-1.5 rounded-full bg-gold-300 animate-ping"></span>
                    <span class="text-[10px] font-semibold tracking-wider uppercase text-gold-200">SMKN 9 Bandung • Perhotelan</span>
                </div>
                
                <div class="space-y-3">
                    <h1 class="text-xs sm:text-sm uppercase tracking-[0.3em] text-slate-400 font-cinzel">Professional Portfolio Of</h1>
                    <h2 class="text-4xl sm:text-5xl xl:text-6xl font-cinzel font-bold text-gold-gradient leading-tight tracking-wider">
                        Muhamad Ali<br class="hidden sm:inline"> Khoirul Rizal
                    </h2>
                </div>
                
                <p class="text-slate-300 max-w-xl text-base sm:text-lg font-light leading-relaxed mx-auto lg:mx-0">
                    Seorang insan hospitality muda yang berdedikasi tinggi, memiliki kedisiplinan fisik prima untuk bekerja keras, jujur, tanggap terhadap situasi lapangan, serta menjunjung tinggi loyalitas perusahaan. Berorientasi pada kesempurnaan pelayanan premium.
                </p>

                <!-- CTA Actions -->
                <div class="flex flex-col sm:flex-row items-center gap-4 pt-4 justify-center lg:justify-start">
                    <a href="https://wa.me/6283159970756" target="_blank" rel="noopener noreferrer" class="w-full sm:w-auto px-8 py-4 bg-gradient-to-r from-gold-500 to-gold-400 hover:from-gold-400 hover:to-gold-300 text-navy-900 font-semibold rounded-xl flex items-center justify-center gap-3 shadow-lg shadow-gold-500/15 transition-all duration-300 transform hover:-translate-y-0.5">
                        <i data-lucide="message-square" class="w-5 h-5"></i>
                        <span>Contact Us (WA)</span>
                    </a>
                    <a href="#ai-interviewer" class="w-full sm:w-auto px-8 py-4 glass-panel border-gold-400/40 hover:bg-gold-400/10 text-gold-300 hover:text-white rounded-xl flex items-center justify-center gap-2 transition-all duration-300">
                        <i data-lucide="sparkles" class="w-5 h-5 text-gold-300"></i>
                        <span>Coba AI Interviewer</span>
                    </a>
                </div>
            </div>

            <!-- RIGHT: Stunning Visual (With your real uploaded photo!) -->
            <div class="lg:col-span-5 flex justify-center order-1 lg:order-2">
                <div class="relative w-72 h-72 sm:w-[380px] sm:h-[380px]">
                    <!-- Outer Halo Glow -->
                    <div class="absolute inset-0 rounded-full bg-gradient-to-br from-gold-400 to-navy-700 p-[2px] opacity-40 animate-pulse"></div>
                    
                    <!-- Decorative Rotating Dash Ring -->
                    <div class="rotating-gold-border"></div>

                    <!-- Inner Photo Canvas Container -->
                    <div class="absolute inset-4 rounded-full overflow-hidden bg-navy-800 border-2 border-gold-300/30 flex items-center justify-center shadow-inner relative z-10 group">
                        
                        <!-- REAL PHOTO - IMG_9590.jpg -->
                        <img src="IMG_9590.jpg" alt="Muhamad Ali Khoirul Rizal" class="w-full h-full object-cover object-center transition-all duration-700 ease-out group-hover:scale-105 filter contrast-[1.02] brightness-[1.05]">
                        
                        <!-- Overlay Glass Effect -->
                        <div class="absolute inset-0 bg-gradient-to-t from-navy-900/60 via-transparent to-transparent opacity-40"></div>
                        <div class="absolute inset-0 border border-white/10 rounded-full pointer-events-none"></div>
                    </div>

                    <!-- Accent Float Tag -->
                    <div class="absolute bottom-4 -right-2 bg-navy-800/90 border border-gold-400/30 backdrop-blur-md rounded-2xl py-2.5 px-4 flex items-center gap-3 shadow-lg z-20">
                        <div class="w-8 h-8 rounded-full bg-gold-400/20 flex items-center justify-center">
                            <i data-lucide="sparkles" class="w-4 h-4 text-gold-300"></i>
                        </div>
                        <div>
                            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-semibold">Spesialis</p>
                            <p class="text-xs font-bold text-gold-200">F&B & Banquet Service</p>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- Personal Overview Section -->
    <section id="about" class="py-24 px-6 relative z-10 bg-navy-800/30 border-y border-gold-400/5">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <h2 class="text-gold-300 font-cinzel text-xs sm:text-sm tracking-[0.3em] uppercase">Eksklusivitas Kepribadian</h2>
                <h3 class="text-2xl sm:text-4xl font-cinzel font-bold text-white">Etos Kerja & Integritas Tinggi</h3>
                <div class="w-16 h-0.5 bg-gold-400 mx-auto mt-4"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Card 1 -->
                <div class="glass-card p-8 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-gold-400/10 border border-gold-400/20 flex items-center justify-center mb-6">
                            <i data-lucide="dumbbell" class="w-5 h-5 text-gold-300"></i>
                        </div>
                        <h4 class="text-lg font-bold font-cinzel text-gold-200 mb-2">Fisik & Stamina Prima</h4>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Memiliki fisik prima, kuat, dan tegap yang ideal untuk menunjang ritme kerja banquet yang dinamis dan bertekanan tinggi secara konsisten.
                        </p>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="glass-card p-8 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-gold-400/10 border border-gold-400/20 flex items-center justify-center mb-6">
                            <i data-lucide="user-check" class="w-5 h-5 text-gold-300"></i>
                        </div>
                        <h4 class="text-lg font-bold font-cinzel text-gold-200 mb-2">Tinggi Rasa Tanggung Jawab</h4>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Setiap amanah dijalankan dengan penuh dedikasi. Menjamin kelancaran operasional servis makanan dari persiapan hingga selesainya acara.
                        </p>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="glass-card p-8 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-gold-400/10 border border-gold-400/20 flex items-center justify-center mb-6">
                            <i data-lucide="eye" class="w-5 h-5 text-gold-300"></i>
                        </div>
                        <h4 class="text-lg font-bold font-cinzel text-gold-200 mb-2">Tanggap Situasi</h4>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Cerdas dalam memetakan keadaan di lapangan. Memiliki kepekaan tinggi untuk membaca kebutuhan tamu secara langsung dan efisien.
                        </p>
                    </div>
                </div>

                <!-- Card 4 -->
                <div class="glass-card p-8 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-gold-400/10 border border-gold-400/20 flex items-center justify-center mb-6">
                            <i data-lucide="shield" class="w-5 h-5 text-gold-300"></i>
                        </div>
                        <h4 class="text-lg font-bold font-cinzel text-gold-200 mb-2">Loyalitas Tanpa Batas</h4>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Berkomitmen tinggi untuk menjaga standar prestise nama besar perusahaan hotel dengan etika kerja profesional yang tulus dan jujur.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-24 px-6 relative z-10">
        <div class="max-w-7xl mx-auto">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Info Section Left -->
                <div class="lg:col-span-4 space-y-6 text-center lg:text-left">
                    <h2 class="text-gold-300 font-cinzel text-xs sm:text-sm tracking-[0.3em] uppercase">Spesialisasi Kompetensi</h2>
                    <h3 class="text-2xl sm:text-4xl font-cinzel font-bold text-white leading-tight">Seni & Keahlian Pelayanan</h3>
                    <div class="w-16 h-0.5 bg-gold-400 mx-auto lg:mx-0"></div>
                    <p class="text-slate-400 text-sm sm:text-base leading-relaxed">
                        Menguasai protokol tata cara hidangan formal secara presisi, menjamin standar estetika serta kenyamanan makan bagi para tamu terhormat.
                    </p>
                </div>

                <!-- Cards Grid Right -->
                <div class="lg:col-span-8 grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <!-- Skill card 1 -->
                    <div class="glass-card p-6 rounded-2xl flex items-start gap-4">
                        <div class="p-3 rounded-lg bg-gold-400/10 border border-gold-400/20 text-gold-300">
                            <i data-lucide="armchair" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h4 class="font-cinzel text-base font-bold text-gold-200 mb-1">Table Manners</h4>
                            <p class="text-xs text-slate-400 leading-relaxed">Sangat memahami etiket makan formal internasional untuk memberikan bimbingan tidak langsung dan melayani tamu.</p>
                        </div>
                    </div>

                    <!-- Skill card 2 -->
                    <div class="glass-card p-6 rounded-2xl flex items-start gap-4">
                        <div class="p-3 rounded-lg bg-gold-400/10 border border-gold-400/20 text-gold-300">
                            <i data-lucide="layout-grid" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h4 class="font-cinzel text-base font-bold text-gold-200 mb-1">Set Up Table</h4>
                            <p class="text-xs text-slate-400 leading-relaxed">Mahir menyusun alat makan (cutlery, glassware, chinaware) dengan penempatan yang presisi sesuai menu.</p>
                        </div>
                    </div>

                    <!-- Skill card 3 -->
                    <div class="glass-card p-6 rounded-2xl flex items-start gap-4">
                        <div class="p-3 rounded-lg bg-gold-400/10 border border-gold-400/20 text-gold-300">
                            <i data-lucide="chef-hat" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h4 class="font-cinzel text-base font-bold text-gold-200 mb-1">F&B Waiter Service</h4>
                            <p class="text-xs text-slate-400 leading-relaxed">Sangat terlatih mengantarkan makanan secara estetik, menyambut tamu, dan memberikan layanan eksklusif.</p>
                        </div>
                    </div>

                    <!-- Skill card 4 -->
                    <div class="glass-card p-6 rounded-2xl flex items-start gap-4">
                        <div class="p-3 rounded-lg bg-gold-400/10 border border-gold-400/20 text-gold-300">
                            <i data-lucide="check-square" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h4 class="font-cinzel text-base font-bold text-gold-200 mb-1">Proper Clear Up</h4>
                            <p class="text-xs text-slate-400 leading-relaxed">Menguasai teknik mengangkat piring kotor tanpa mengganggu kenyamanan mengobrol para pelanggan di meja.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Timeline Section -->
    <section id="experience" class="py-24 px-6 relative z-10 bg-navy-800/30 border-t border-gold-400/5">
        <div class="max-w-5xl mx-auto">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <h2 class="text-gold-300 font-cinzel text-xs sm:text-sm tracking-[0.3em] uppercase">Rekam Jejak Operasional</h2>
                <h3 class="text-2xl sm:text-4xl font-cinzel font-bold text-white">Pengalaman Kerja Eksklusif</h3>
                <div class="w-16 h-0.5 bg-gold-400 mx-auto mt-4"></div>
            </div>

            <!-- Timeline -->
            <div class="relative border-l border-gold-400/20 ml-4 md:ml-32 space-y-12">
                
                <!-- Experience Item 1 -->
                <div class="relative pl-8 sm:pl-12">
                    <!-- Dot Accent -->
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-navy-800 border-2 border-gold-400 flex items-center justify-center">
                        <span class="w-1.5 h-1.5 rounded-full bg-gold-400"></span>
                    </div>

                    <!-- Year/Label on Left for large screen -->
                    <div class="hidden md:block absolute -left-32 top-1.5 w-24 text-right text-xs uppercase tracking-widest text-gold-300 font-semibold">
                        Praktik SMK
                    </div>

                    <div class="glass-card p-6 sm:p-8 rounded-2xl relative">
                        <span class="absolute top-4 right-4 bg-gold-400/10 border border-gold-400/20 text-gold-300 text-[10px] px-3 py-1 rounded-full font-bold uppercase tracking-wider">
                            20+ Kali Praktik
                        </span>
                        
                        <div class="flex items-center gap-3 mb-4">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold-300 flex-shrink-0"></i>
                            <div>
                                <h4 class="text-lg sm:text-xl font-cinzel font-bold text-white">InterContinental Bandung Dago Pakar</h4>
                                <p class="text-xs text-slate-400 uppercase tracking-widest mt-0.5">F&B Service / Waiter</p>
                            </div>
                        </div>

                        <p class="text-slate-300 text-sm leading-relaxed mb-4">
                            Telah melakukan praktik secara intensif sebanyak kurang lebih 20 kali di InterContinental Bandung. Memiliki keahlian mendalam sebagai *waiter* yang profesional, memahami kaidah pemberian makanan yang elegan kepada tamu secara higienis dan benar, serta terampil melakukan proses *clear-up* secara taktis dan rapi.
                        </p>
                    </div>
                </div>

                <!-- Experience Item 2 -->
                <div class="relative pl-8 sm:pl-12">
                    <!-- Dot Accent -->
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-navy-800 border-2 border-gold-400 flex items-center justify-center">
                        <span class="w-1.5 h-1.5 rounded-full bg-gold-400"></span>
                    </div>

                    <!-- Year/Label on Left for large screen -->
                    <div class="hidden md:block absolute -left-32 top-1.5 w-24 text-right text-xs uppercase tracking-widest text-gold-300 font-semibold">
                        Kerja Casual
                    </div>

                    <div class="glass-card p-6 sm:p-8 rounded-2xl relative">
                        <span class="absolute top-4 right-4 bg-gold-400/10 border border-gold-400/20 text-gold-300 text-[10px] px-3 py-1 rounded-full font-bold uppercase tracking-wider">
                            7 Kali Kasual
                        </span>
                        
                        <div class="flex items-center gap-3 mb-4">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold-300 flex-shrink-0"></i>
                            <div>
                                <h4 class="text-lg sm:text-xl font-cinzel font-bold text-white">Hotel Indigo Bandung Dago Pakar</h4>
                                <p class="text-xs text-slate-400 uppercase tracking-widest mt-0.5">Banquet Service Department</p>
                            </div>
                        </div>

                        <p class="text-slate-300 text-sm leading-relaxed mb-4">
                            Mendapatkan kepercayaan penuh sebanyak 7 kali dalam tim operasional Banquet Service. Berkontribusi langsung dalam menyiapkan, melayani, dan merapikan ruangan pertemuan berskala VIP, *wedding event*, serta kegiatan korporat berkelas tinggi.
                        </p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ✨ GEMINI AI SECTION: Interactive Hospitality Assistant & Interview Simulator -->
    <section id="ai-interviewer" class="py-24 px-6 relative z-10 bg-navy-950/80 border-t border-gold-400/10">
        <div class="max-w-4xl mx-auto">
            <!-- Header -->
            <div class="text-center max-w-2xl mx-auto mb-12 space-y-3">
                <div class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full bg-gold-400/10 border border-gold-400/30 text-gold-300 text-xs font-semibold">
                    <i data-lucide="sparkles" class="w-3.5 h-3.5 text-gold-300"></i>
                    <span>Ditenagai Gemini 2.5 Flash</span>
                </div>
                <h3 class="text-2xl sm:text-4xl font-cinzel font-bold text-white">✨ AI Interviewer & Assistant</h3>
                <p class="text-xs text-slate-400 tracking-widest uppercase">Uji kompetensi Ali secara instan di sini</p>
                <div class="w-16 h-0.5 bg-gold-400 mx-auto mt-4"></div>
            </div>

            <!-- Main Interface Layout -->
            <div class="glass-panel rounded-3xl overflow-hidden border border-gold-400/20 shadow-2xl flex flex-col md:grid md:grid-cols-12 h-[550px]">
                
                <!-- Info & Modes Panel (3/12 wide on desktop) -->
                <div class="md:col-span-4 bg-navy-900/60 p-6 border-b md:border-b-0 md:border-r border-gold-400/10 flex flex-col justify-between">
                    <div>
                        <h4 class="font-cinzel text-sm font-bold text-gold-300 mb-3 tracking-wider">PILIH MODE ASISTEN</h4>
                        <p class="text-[11px] text-slate-400 mb-6 leading-relaxed">Gunakan simulasi interaktif ini untuk mewawancarai Ali Rizal atau menanyakan detail pengalamannya secara otomatis.</p>
                        
                        <!-- Toggle Buttons -->
                        <div class="space-y-3">
                            <button id="modeAssistantBtn" class="w-full text-left p-3 rounded-xl border border-gold-400 bg-gold-400/10 text-gold-200 text-xs font-semibold flex items-center gap-2.5 transition-all">
                                <i data-lucide="user-cog" class="w-4 h-4 text-gold-300"></i>
                                <span>Tanya Profil Ali</span>
                            </button>
                            <button id="modeInterviewerBtn" class="w-full text-left p-3 rounded-xl border border-gold-400/10 hover:border-gold-400/40 hover:bg-navy-800 text-slate-400 hover:text-slate-200 text-xs font-semibold flex items-center gap-2.5 transition-all">
                                <i data-lucide="graduation-cap" class="w-4 h-4 text-slate-400"></i>
                                <span>✨ Simulasi Wawancara</span>
                            </button>
                        </div>
                    </div>

                    <!-- Quick Prompts / Icebreakers -->
                    <div class="hidden md:block pt-6">
                        <span class="text-[10px] text-slate-500 uppercase tracking-wider block mb-2 font-semibold">Saran Pertanyaan:</span>
                        <div class="space-y-2 text-[11px]">
                            <button onclick="fillPrompt('Ceritakan pengalaman kerja casual kamu di Hotel Indigo')" class="block w-full text-left p-2 rounded-lg bg-navy-800/40 hover:bg-navy-800 border border-white/5 text-slate-300 hover:text-gold-200 transition-colors truncate">
                                💬 Pengalaman Hotel Indigo Dago
                            </button>
                            <button onclick="fillPrompt('Bagaimana cara Ali menyajikan hidangan dan melakukan clear up?')" class="block w-full text-left p-2 rounded-lg bg-navy-800/40 hover:bg-navy-800 border border-white/5 text-slate-300 hover:text-gold-200 transition-colors truncate">
                                🍽️ Teknik Service & Clear Up
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Chat Area (8/12 wide on desktop) -->
                <div class="md:col-span-8 flex flex-col h-full bg-navy-950/40 relative">
                    <!-- Chat Header -->
                    <div class="px-6 py-4 border-b border-gold-400/10 bg-navy-900/40 flex items-center justify-between">
                        <div class="flex items-center gap-2.5">
                            <div class="w-2.5 h-2.5 rounded-full bg-emerald-500 animate-pulse"></div>
                            <span id="chatHeaderStatus" class="text-xs font-semibold tracking-wider text-slate-300">Asisten Profil Ali (Aktif)</span>
                        </div>
                        <button onclick="resetChat()" class="text-slate-500 hover:text-gold-300 transition-colors text-[11px] flex items-center gap-1">
                            <i data-lucide="rotate-ccw" class="w-3.5 h-3.5"></i> Reset Chat
                        </button>
                    </div>

                    <!-- Chat Messages Log Container -->
                    <div id="chatMessages" class="flex-1 overflow-y-auto p-6 space-y-4 text-xs sm:text-sm">
                        <!-- Bot Welcome Message -->
                        <div class="flex gap-3 max-w-[85%]">
                            <div class="w-8 h-8 rounded-full bg-gold-400/10 border border-gold-400/30 flex items-center justify-center flex-shrink-0 text-gold-300">
                                <i data-lucide="sparkles" class="w-4 h-4"></i>
                            </div>
                            <div class="bg-navy-800/80 border border-white/5 rounded-2xl p-3.5 text-slate-300 leading-relaxed">
                                <p id="welcomeText">Halo! Saya adalah AI Assistant milik Ali Rizal. Anda bisa menanyakan apa saja mengenai pengalaman Banquet Service saya di Hotel Indigo, praktek F&B di InterContinental, maupun keahlian Table Manners saya. Silakan kirim pertanyaan Anda!</p>
                            </div>
                        </div>
                    </div>

                    <!-- Chat Input -->
                    <form id="chatForm" class="p-4 border-t border-gold-400/10 bg-navy-900/40 flex gap-2">
                        <input type="text" id="userInput" placeholder="Ketik pertanyaan Anda tentang kompetensi Ali..." class="flex-grow bg-navy-900/80 border border-gold-400/20 hover:border-gold-400/40 focus:border-gold-400 rounded-xl px-4 py-3 text-xs sm:text-sm text-slate-200 placeholder-slate-500 focus:outline-none transition-all">
                        <button type="submit" id="sendBtn" class="bg-gradient-to-r from-gold-500 to-gold-400 text-navy-900 px-5 py-3 rounded-xl hover:from-gold-400 hover:to-gold-300 font-bold transition-all flex items-center justify-center gap-1.5 flex-shrink-0">
                            <span class="hidden sm:inline">Kirim</span>
                            <i data-lucide="send" class="w-4 h-4"></i>
                        </button>
                    </form>
                </div>

            </div>
        </div>
    </section>

    <!-- Floating Action Quote (Interactive) -->
    <section class="py-12 px-6 relative z-10">
        <div class="max-w-4xl mx-auto glass-panel p-8 sm:p-12 rounded-3xl border border-gold-400/20 text-center relative overflow-hidden">
            <div class="absolute -top-12 -left-12 w-48 h-48 bg-gold-400/5 rounded-full filter blur-xl"></div>
            <div class="absolute -bottom-12 -right-12 w-48 h-48 bg-navy-600/20 rounded-full filter blur-xl"></div>

            <i data-lucide="quote" class="w-10 h-10 text-gold-300/30 mx-auto mb-6"></i>
            <h3 class="font-cinzel text-lg sm:text-2xl text-gold-200 leading-relaxed italic mb-8">
                "Kualitas layanan terbaik terletak pada perhatian terhadap detail-detail kecil yang tidak terlihat, namun sangat dirasakan oleh tamu."
            </h3>

            <!-- Dynamic CTA Button with Ripple -->
            <a href="https://wa.me/6283159970756" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-3 bg-gradient-to-r from-gold-500 to-gold-400 hover:from-gold-400 hover:to-gold-300 text-navy-900 font-semibold px-8 py-4 rounded-xl shadow-lg transition-all duration-300 hover:shadow-gold-400/20 transform hover:-translate-y-0.5">
                <i data-lucide="phone" class="w-5 h-5"></i>
                <span>Hubungi Saya untuk Sesi Casual / Interview</span>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-navy-900 border-t border-gold-400/10 py-12 px-6 relative z-10 text-slate-400">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6">
            <!-- Brand -->
            <div class="flex items-center gap-3">
                <i data-lucide="hotel" class="w-6 h-6 text-gold-300"></i>
                <div class="text-left">
                    <p class="font-cinzel text-sm font-bold tracking-widest text-gold-300">A. RIZAL</p>
                    <p class="text-[9px] uppercase tracking-[0.2em] text-slate-500">Hospitality Portfolio</p>
                </div>
            </div>

            <p class="text-center text-xs text-slate-500">
                &copy; 2026 Muhamad Ali Khoirul Rizal. All Rights Reserved.
            </p>

            <!-- Back to top trigger -->
            <a href="#" class="p-3 bg-navy-800 hover:bg-navy-700 border border-gold-400/10 hover:border-gold-400/30 rounded-xl transition-all duration-300 text-gold-300" aria-label="Kembali ke atas">
                <i data-lucide="arrow-up" class="w-4 h-4"></i>
            </a>
        </div>
    </footer>

    <!-- Interactive JS Core & Gemini API Integration -->
    <script>
        // Init Lucide Icons
        lucide.createIcons();

        // DOM elements for Navigation Drawer
        const menuBtn = document.getElementById('menuBtn');
        const sideMenu = document.getElementById('sideMenu');
        const drawerContent = document.getElementById('drawerContent');
        const line1 = document.getElementById('line1');
        const line2 = document.getElementById('line2');
        const line3 = document.getElementById('line3');
        const mainHeader = document.getElementById('mainHeader');

        let isMenuOpen = false;

        // Toggle Drawer Function
        function toggleMenu() {
            isMenuOpen = !isMenuOpen;
            if (isMenuOpen) {
                sideMenu.classList.remove('opacity-0', 'pointer-events-none');
                sideMenu.classList.add('opacity-100');
                drawerContent.classList.remove('translate-x-full');
                
                line1.style.transform = 'rotate(45deg) translate(5px, 5px)';
                line2.style.opacity = '0';
                line3.style.transform = 'rotate(-45deg) translate(5px, -5px)';
            } else {
                sideMenu.classList.remove('opacity-100');
                sideMenu.classList.add('opacity-0', 'pointer-events-none');
                drawerContent.classList.add('translate-x-full');

                line1.style.transform = 'none';
                line2.style.opacity = '1';
                line3.style.transform = 'none';
            }
        }

        menuBtn.addEventListener('click', toggleMenu);
        sideMenu.addEventListener('click', (e) => {
            if (e.target === sideMenu) {
                toggleMenu();
            }
        });

        // Sticky Navbar effect on Scroll
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                mainHeader.classList.add('bg-navy-900/90', 'backdrop-blur-md', 'shadow-lg', 'border-b', 'border-gold-400/10');
            } else {
                mainHeader.classList.remove('bg-navy-900/90', 'backdrop-blur-md', 'shadow-lg', 'border-b', 'border-gold-400/10');
            }
        });


        /* ==========================================================================
           ✨ GEMINI 2.5 FLASH LLM INTEGRATION
           ========================================================================== */
        
        // Empty string API key. The runtime environment provides the key automatically.
        const apiKey = "";
        const apiEndpoint = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`;

        // Chat Status Variables
        let currentMode = 'assistant'; // 'assistant' atau 'interviewer'
        let chatHistory = [];

        // UI DOM elements for AI
        const modeAssistantBtn = document.getElementById('modeAssistantBtn');
        const modeInterviewerBtn = document.getElementById('modeInterviewerBtn');
        const chatHeaderStatus = document.getElementById('chatHeaderStatus');
        const welcomeText = document.getElementById('welcomeText');
        const chatMessages = document.getElementById('chatMessages');
        const chatForm = document.getElementById('chatForm');
        const userInput = document.getElementById('userInput');
        const sendBtn = document.getElementById('sendBtn');

        // Ali Rizal's Resume Data Injector for LLM Context
        const aliDataProfile = `
        BERIKUT ADALAH PROFIL RESMI PEMILIK PORTFOLIO:
        - Nama Lengkap: Muhamad Ali Khoirul Rizal
        - Tempat/Tanggal Lahir: Lampung, 17 Desember 2009
        - Pendidikan: Pelajar aktif di SMKN 9 Bandung (Jurusan Perhotelan / Hospitality)
        - Etos & Fisik: Memiliki fisik yang tangguh, kuat, postur ideal untuk bekerja keras di perhotelan khususnya banquet/F&B service. Jujur, bertanggung jawab, tanggap terhadap situasi lapangan, serta sangat loyal kepada perusahaan tempat bekerja.
        - Pengalaman Kerja Casual:
          * Hotel Indigo Bandung Dago Pakar (7 Kali ditempatkan di divisi Banquet Service)
        - Pengalaman Praktik Sekolah:
          * InterContinental Bandung Dago Pakar (Kurang lebih 20 kali praktik di divisi F&B Service sebagai Waiter)
        - Keahlian Khusus:
          * Sangat mahir dalam Table Manners standar internasional.
          * Sangat mahir menyusun susunan alat makan formal (Set up table).
          * Memahami cara membawakan/menyajikan makanan kepada tamu hotel bintang lima dengan benar dan berkelas.
          * Memahami teknik "clear up" (mengangkat alat makan kotor) dengan taktis, halus, dan rapi tanpa mengganggu tamu.
        - Kontak Langsung: WhatsApp (https://wa.me/6283159970756) atau nomor HP (+62 831-5997-0756)
        `;

        // System Instruction Prompts based on Mode
        const systemPromptAssistant = `
        Anda adalah Asisten Profil AI pribadi yang elegan dari Muhamad Ali Khoirul Rizal.
        Tugas Anda adalah menjawab pertanyaan HRD, manager hotel, atau pengunjung website mengenai data diri, keahlian, dan kepribadian Ali secara sopan, ramah, dan sangat profesional dengan gaya bahasa industri perhotelan bintang lima (Gunakan sapaan sopan seperti Bapak/Ibu).
        Gunakan data profil Ali berikut sebagai satu-satunya acuan kebenaran fakta:
        ${aliDataProfile}
        Gunakan bahasa Indonesia yang baik, elegan, dan menonjolkan kelebihan Ali tanpa berlebihan. Jangan membuat fakta palsu yang tidak ada dalam profil Ali.
        `;

        const systemPromptInterviewer = `
        Anda berperan sebagai HR Director atau Food & Beverage Director dari sebuah Hotel Mewah Bintang 5 Internasional (seperti InterContinental, Ritz-Carlton, atau Indigo).
        Tugas Anda adalah mewawancarai Muhamad Ali Khoirul Rizal secara langsung.
        Posisikan pengguna yang sedang chat dengan Anda sebagai Ali Rizal. Ajukan pertanyaan-pertanyaan wawancara kerja F&B, Banquet, atau Service yang menantang secara bergantian satu per satu.
        Beri penilaian objektif yang sopan pada jawaban Ali, lalu lanjutkan dengan pertanyaan wawancara berikutnya.
        Mulai dengan salam hangat, sapa Ali dengan ramah, dan ajukan pertanyaan wawancara pertama tentang kesiapan fisiknya, pengalamannya di Hotel Indigo/InterContinental, atau keahlian teknisnya.
        Berikut adalah resume Ali sebagai acuan Anda saat bertanya:
        ${aliDataProfile}
        Gunakan gaya bicara HRD profesional hotel yang ramah namun berwibawa dan berorientasi pada detail layanan premium.
        `;

        // Toggle Modes Event Listeners
        modeAssistantBtn.addEventListener('click', () => {
            setMode('assistant');
        });

        modeInterviewerBtn.addEventListener('click', () => {
            setMode('interviewer');
        });

        function setMode(mode) {
            currentMode = mode;
            resetChat();
            
            if (mode === 'assistant') {
                // Style Active State for Assistant
                modeAssistantBtn.classList.add('border-gold-400', 'bg-gold-400/10', 'text-gold-200');
                modeAssistantBtn.classList.remove('border-gold-400/10', 'text-slate-400');
                modeInterviewerBtn.classList.remove('border-gold-400', 'bg-gold-400/10', 'text-gold-200');
                modeInterviewerBtn.classList.add('border-gold-400/10', 'text-slate-400');
                
                chatHeaderStatus.innerText = "Asisten Profil Ali (Aktif)";
                welcomeText.innerText = "Halo! Saya adalah AI Assistant milik Ali Rizal. Anda bisa menanyakan apa saja mengenai pengalaman Banquet Service saya di Hotel Indigo, praktek F&B di InterContinental, maupun keahlian Table Manners saya. Silakan kirim pertanyaan Anda!";
                userInput.placeholder = "Ketik pertanyaan Anda tentang kompetensi Ali...";
            } else {
                // Style Active State for Interviewer
                modeInterviewerBtn.classList.add('border-gold-400', 'bg-gold-400/10', 'text-gold-200');
                modeInterviewerBtn.classList.remove('border-gold-400/10', 'text-slate-400');
                modeAssistantBtn.classList.remove('border-gold-400', 'bg-gold-400/10', 'text-gold-200');
                modeAssistantBtn.classList.add('border-gold-400/10', 'text-slate-400');
                
                chatHeaderStatus.innerText = "✨ Mode Simulasi Wawancara";
                welcomeText.innerText = "Selamat datang di Simulasi Wawancara Kerja. Saya akan bertindak sebagai Food & Beverage Director Hotel Bintang 5. Anggap diri Anda sebagai Ali Rizal dan jawablah pertanyaan saya seserius mungkin. Mari kita mulai!";
                userInput.placeholder = "Jawablah pertanyaan interview di sini...";
                
                // Trigger First Interview Question from Gemini
                triggerFirstInterviewerQuestion();
            }
        }

        function fillPrompt(text) {
            userInput.value = text;
            userInput.focus();
        }

        function resetChat() {
            chatMessages.innerHTML = `
                <div class="flex gap-3 max-w-[85%]">
                    <div class="w-8 h-8 rounded-full bg-gold-400/10 border border-gold-400/30 flex items-center justify-center flex-shrink-0 text-gold-300">
                        <i data-lucide="sparkles" class="w-4 h-4"></i>
                    </div>
                    <div class="bg-navy-800/80 border border-white/5 rounded-2xl p-3.5 text-slate-300 leading-relaxed">
                        <p id="welcomeText">${welcomeText.innerText}</p>
                    </div>
                </div>
            `;
            chatHistory = [];
            lucide.createIcons();
        }

        // Trigger First Interviewer Question
        async function triggerFirstInterviewerQuestion() {
            appendLoadingIndicator();
            const response = await callGeminiAPI("Mulai wawancara dan sapa calon pelamar (Ali Rizal) lalu ajukan pertanyaan pertama.");
            removeLoadingIndicator();
            appendMessage('bot', response);
        }

        // Append Single Message to UI Bubble Log
        function appendMessage(sender, text) {
            const wrapper = document.createElement('div');
            wrapper.className = sender === 'user' ? 'flex justify-end' : 'flex gap-3 max-w-[85%]';
            
            if (sender === 'user') {
                wrapper.innerHTML = `
                    <div class="bg-gold-400/15 border border-gold-400/30 rounded-2xl p-3.5 text-gold-200 max-w-[85%] leading-relaxed">
                        <p>${escapeHTML(text)}</p>
                    </div>
                `;
            } else {
                wrapper.innerHTML = `
                    <div class="w-8 h-8 rounded-full bg-gold-400/10 border border-gold-400/30 flex items-center justify-center flex-shrink-0 text-gold-300">
                        <i data-lucide="sparkles" class="w-4 h-4"></i>
                    </div>
                    <div class="bg-navy-800/80 border border-white/5 rounded-2xl p-3.5 text-slate-300 leading-relaxed">
                        <p>${text.replace(/\n/g, '<br>')}</p>
                    </div>
                `;
            }
            chatMessages.appendChild(wrapper);
            chatMessages.scrollTop = chatMessages.scrollHeight;
            lucide.createIcons();
        }

        function appendLoadingIndicator() {
            const wrapper = document.createElement('div');
            wrapper.id = 'geminiLoading';
            wrapper.className = 'flex gap-3 max-w-[85%]';
            wrapper.innerHTML = `
                <div class="w-8 h-8 rounded-full bg-gold-400/10 border border-gold-400/30 flex items-center justify-center flex-shrink-0 text-gold-300">
                    <i data-lucide="loader-2" class="w-4 h-4 animate-spin"></i>
                </div>
                <div class="bg-navy-800/50 border border-white/5 rounded-2xl p-3.5 text-slate-400 italic">
                    Sedang berpikir...
                </div>
            `;
            chatMessages.appendChild(wrapper);
            chatMessages.scrollTop = chatMessages.scrollHeight;
            lucide.createIcons();
        }

        function removeLoadingIndicator() {
            const element = document.getElementById('geminiLoading');
            if (element) element.remove();
        }

        function escapeHTML(str) {
            return str.replace(/[&<>'"]/g, 
                tag => ({ '&': '&amp;', '<': '&lt;', '>': '&gt;', "'": '&#39;', '"': '&quot;' }[tag] || tag)
            );
        }

        // Core Call to Gemini API (with 5x exponential backoff retry)
        async function callGeminiAPI(promptText) {
            const systemPrompt = currentMode === 'assistant' ? systemPromptAssistant : systemPromptInterviewer;
            
            // Build Contextual Contents payload including brief chat logs
            const contents = [];
            
            // Limit history context to last 6 exchanges to maintain fast token responses
            const recentHistory = chatHistory.slice(-6);
            recentHistory.forEach(item => {
                contents.push({
                    role: item.role,
                    parts: [{ text: item.text }]
                });
            });

            // Append current prompt text
            contents.push({
                role: "user",
                parts: [{ text: promptText }]
            });

            const payload = {
                contents: contents,
                systemInstruction: {
                    parts: [{ text: systemPrompt }]
                }
            };

            let delay = 1000;
            for (let i = 0; i < 5; i++) {
                try {
                    const response = await fetch(apiEndpoint, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (!response.ok) throw new Error(`HTTP Error ${response.status}`);
                    
                    const result = await response.json();
                    const aiResponse = result.candidates?.[0]?.content?.parts?.[0]?.text;
                    
                    if (aiResponse) {
                        // Store exchange in local history log
                        chatHistory.push({ role: 'user', text: promptText });
                        chatHistory.push({ role: 'model', text: aiResponse });
                        return aiResponse;
                    } else {
                        throw new Error("Respons teks kosong dari Gemini API.");
                    }

                } catch (error) {
                    if (i === 4) { // Final retry failed
                        return "Maaf sekali, sistem asisten AI kami sedang mengalami kendala koneksi atau batas kuota harian terlampaui. Silakan coba kembali sesaat lagi atau langsung hubungi saya melalui WhatsApp!";
                    }
                    await new Promise(resolve => setTimeout(resolve, delay));
                    delay *= 2; // Exponential Backoff
                }
            }
        }

        // Form Submission Event
        chatForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            const text = userInput.value.trim();
            if (!text) return;

            // Clear input box
            userInput.value = '';

            // Render user bubble
            appendMessage('user', text);

            // Fetch Gemini Response
            appendLoadingIndicator();
            const aiResponseText = await callGeminiAPI(text);
            removeLoadingIndicator();

            // Render Bot Response
            appendMessage('bot', aiResponseText);
        });
    </script>
</body>
	</html>
