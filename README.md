<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mayank Chandrakapure | B.Tech Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter & Outfit -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Outfit:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Outfit', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            400: '#38bdf8',
                            500: '#0ea5e9',
                            600: '#0284c7',
                            900: '#0c4a6e',
                        }
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #080c14;
            color: #f3f4f6;
            overflow-x: hidden;
        }

        .glass-card {
            background: rgba(17, 24, 39, 0.7);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }

        .glass-card:hover {
            border-color: rgba(56, 189, 248, 0.3);
            box-shadow: 0 10px 30px -10px rgba(14, 165, 233, 0.25);
        }

        .gradient-text {
            background: linear-gradient(135deg, #38bdf8 0%, #818cf8 50%, #c084fc 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .glow-effect {
            box-shadow: 0 0 40px -5px rgba(56, 189, 248, 0.4);
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #080c14;
        }
        ::-webkit-scrollbar-thumb {
            background: #1f2937;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #0ea5e9;
        }
    </style>
</head>
<body class="antialiased selection:bg-brand-500 selection:text-white">

    <header class="fixed top-0 left-0 w-full z-50 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Logo -->
                <a href="#" class="font-heading font-bold text-xl sm:text-2xl tracking-tight text-white flex items-center gap-2">
                    <span class="w-9 h-9 rounded-xl bg-gradient-to-tr from-brand-500 to-indigo-500 flex items-center justify-center text-white font-black shadow-lg shadow-brand-500/30">M</span>
                    <span>Mayank<span class="text-brand-400">.</span></span>
                </a>

                <!-- Desktop Links -->
                <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
                    <a href="#about" class="hover:text-brand-400 transition-colors duration-200">About</a>
                    <a href="#education" class="hover:text-brand-400 transition-colors duration-200">Education</a>
                    <a href="#skills" class="hover:text-brand-400 transition-colors duration-200">Skills</a>
                    <a href="#contact" class="hover:text-brand-400 transition-colors duration-200">Contact</a>
                </nav>

                <!-- Phone CTA -->
                <div class="hidden md:flex items-center gap-4">
                    <a href="tel:+917499491802" class="px-5 py-2.5 rounded-full bg-brand-500/10 border border-brand-500/30 text-brand-400 hover:bg-brand-500 hover:text-white text-sm font-semibold transition-all duration-300 flex items-center gap-2">
                        <i class="fa-solid fa-phone text-xs"></i> Call Me
                    </a>
                </div>

                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" class="md:hidden text-gray-300 hover:text-white focus:outline-none p-2">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden glass-card border-t border-gray-800 px-6 py-6 space-y-4">
            <a href="#about" class="block text-gray-300 hover:text-brand-400 font-medium py-2">About</a>
            <a href="#education" class="block text-gray-300 hover:text-brand-400 font-medium py-2">Education</a>
            <a href="#skills" class="block text-gray-300 hover:text-brand-400 font-medium py-2">Skills</a>
            <a href="#contact" class="block text-gray-300 hover:text-brand-400 font-medium py-2">Contact</a>
            <div class="pt-2">
                <a href="tel:+917499491802" class="w-full text-center px-5 py-3 rounded-xl bg-brand-500 text-white font-semibold inline-block">
                    <i class="fa-solid fa-phone mr-2"></i> +91 7499491802
                </a>
            </div>
        </div>
    </header>

    <section class="relative pt-32 pb-20 md:pt-40 md:pb-32 overflow-hidden flex items-center min-h-screen">
        <div class="absolute top-1/4 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[500px] bg-brand-500/15 rounded-full blur-[120px] pointer-events-none"></div>
        <div class="absolute bottom-10 right-10 w-[300px] h-[300px] bg-indigo-500/10 rounded-full blur-[100px] pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 w-full">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
                
                <!-- Left Introduction -->
                <div class="lg:col-span-7 text-center lg:text-left space-y-6">
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full glass-card border border-brand-500/20 text-brand-400 text-sm font-medium">
                        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span>
                        Available for Opportunities
                    </div>

                    <h1 class="font-heading text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-tight text-white">
                        Hello, I'm <br class="hidden sm:inline"/>
                        <span class="gradient-text">Mayank Chandrakapure</span>
                    </h1>

                    <p class="text-lg sm:text-xl text-gray-300 max-w-2xl font-light">
                        A passionate <strong class="text-white font-semibold">20-Year-Old B.Tech Engineering Student</strong> at S B Jain Institute of Technology, Research and Management, Nagpur. Building a solid foundation for a successful career in technology.
                    </p>

                    <!-- Key Badges -->
                    <div class="flex flex-wrap items-center justify-center lg:justify-start gap-3 pt-2">
                        <div class="px-3.5 py-1.5 rounded-lg bg-gray-800/80 border border-gray-700/60 text-xs font-semibold text-gray-300 flex items-center gap-2">
                            <i class="fa-solid fa-graduation-cap text-brand-400"></i> B.Tech Student
                        </div>
                        <div class="px-3.5 py-1.5 rounded-lg bg-gray-800/80 border border-gray-700/60 text-xs font-semibold text-gray-300 flex items-center gap-2">
                            <i class="fa-solid fa-user text-indigo-400"></i> 20 Years Old
                        </div>
                        <div class="px-3.5 py-1.5 rounded-lg bg-gray-800/80 border border-gray-700/60 text-xs font-semibold text-gray-300 flex items-center gap-2">
                            <i class="fa-solid fa-location-dot text-rose-400"></i> Nagpur, MH
                        </div>
                    </div>

                    <!-- Call To Action Buttons -->
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
                        <a href="https://www.linkedin.com/in/mayank-chandrakapure-3b8a68383" target="_blank" rel="noopener noreferrer" class="w-full sm:w-auto px-8 py-3.5 rounded-xl bg-gradient-to-r from-brand-500 to-indigo-600 hover:from-brand-600 hover:to-indigo-700 text-white font-semibold shadow-lg shadow-brand-500/25 transition-all duration-300 flex items-center justify-center gap-3">
                            <i class="fa-brands fa-linkedin text-lg"></i> Connect on LinkedIn
                        </a>
                        <a href="#contact" class="w-full sm:w-auto px-8 py-3.5 rounded-xl glass-card text-gray-200 hover:text-white hover:border-brand-500/50 font-semibold transition-all duration-300 flex items-center justify-center gap-2">
                            Get In Touch <i class="fa-solid fa-arrow-right text-xs"></i>
                        </a>
                    </div>
                </div>

                <!-- Right Profile Image with SVG Graphic Fallback -->
                <div class="lg:col-span-5 flex justify-center">
                    <div class="relative group">
                        <div class="absolute -inset-1 bg-gradient-to-r from-brand-500 to-indigo-500 rounded-full blur-xl opacity-50 group-hover:opacity-80 transition duration-500"></div>
                        
                        <div class="relative w-64 h-64 sm:w-80 sm:h-80 md:w-88 md:h-88 rounded-full p-2 bg-gradient-to-tr from-brand-500 via-indigo-500 to-purple-500 glow-effect">
                            <div class="w-full h-full rounded-full overflow-hidden bg-gray-900 border-4 border-gray-900 relative flex items-center justify-center">
                                <!-- Profile Graphic SVG -->
                                <svg class="w-full h-full text-brand-400 p-2" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <circle cx="100" cy="100" r="96" fill="#0f172a" stroke="#0ea5e9" stroke-width="4"/>
                                    <circle cx="100" cy="70" r="38" fill="#38bdf8"/>
                                    <path d="M30 170C30 135 60 120 100 120C140 120 170 135 170 170V190H30V170Z" fill="#0284c7"/>
                                    <circle cx="85" cy="65" r="5" fill="#090d16"/>
                                    <circle cx="115" cy="65" r="5" fill="#090d16"/>
                                    <path d="M85 85Q100 95 115 85" stroke="#090d16" stroke-width="3" stroke-linecap="round"/>
                                </svg>
                            </div>
                        </div>

                        <!-- Badge Overlay -->
                        <div class="absolute -bottom-2 -left-2 glass-card px-4 py-2.5 rounded-2xl border border-gray-700/80 shadow-xl flex items-center gap-3">
                            <div class="w-10 h-10 rounded-xl bg-emerald-500/10 text-emerald-400 flex items-center justify-center">
                                <i class="fa-solid fa-building-columns text-lg"></i>
                            </div>
                            <div>
                                <p class="text-[10px] uppercase tracking-wider text-gray-400 font-medium">Institution</p>
                                <p class="text-xs font-bold text-white">S B Jain, Nagpur</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <section id="about" class="py-20 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-semibold text-brand-400 tracking-widest uppercase mb-2">Personal Overview</h2>
                <h3 class="font-heading text-3xl sm:text-4xl font-bold text-white">About Me</h3>
                <div class="w-12 h-1 bg-brand-500 mx-auto rounded-full mt-4"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Bio Card -->
                <div class="md:col-span-2 glass-card rounded-2xl p-8 border border-gray-800">
                    <h4 class="font-heading text-2xl font-bold text-white mb-4">Engineering Student & Tech Enthusiast</h4>
                    <p class="text-gray-300 leading-relaxed mb-6">
                        I am <strong class="text-white">Mayank Jagjiwan Chandrakapure</strong>, a 20-year-old engineering student residing in Nagpur, Maharashtra. Currently, I am pursuing my Bachelor of Technology (B.Tech) degree at S B Jain Institute of Technology, Research and Management.
                    </p>
                    <p class="text-gray-300 leading-relaxed mb-6">
                        I am deeply passionate about expanding my knowledge in engineering concepts, technological solutions, and practical project development. Having completed my Higher Secondary Education with a 71% score at St. Paul College, I am focused on combining academic excellence with hands-on technical skills.
                    </p>

                    <div class="grid grid-cols-2 sm:grid-cols-3 gap-4 pt-4 border-t border-gray-800">
                        <div>
                            <span class="text-gray-400 text-xs uppercase block">Full Name</span>
                            <span class="text-white text-sm font-semibold">Mayank Chandrakapure</span>
                        </div>
                        <div>
                            <span class="text-gray-400 text-xs uppercase block">Age</span>
                            <span class="text-white text-sm font-semibold">20 Years</span>
                        </div>
                        <div>
                            <span class="text-gray-400 text-xs uppercase block">Location</span>
                            <span class="text-white text-sm font-semibold">Nagpur, India</span>
                        </div>
                    </div>
                </div>

                <!-- Info Sidebar -->
                <div class="glass-card rounded-2xl p-8 border border-gray-800 flex flex-col justify-between space-y-6">
                    <div>
                        <h4 class="font-heading text-xl font-bold text-white mb-4">Quick Details</h4>
                        <ul class="space-y-4">
                            <li class="flex items-start gap-3">
                                <div class="w-8 h-8 rounded-lg bg-brand-500/10 text-brand-400 flex items-center justify-center shrink-0 mt-0.5">
                                    <i class="fa-solid fa-graduation-cap text-sm"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-gray-400">Current Degree</p>
                                    <p class="text-sm font-semibold text-white">B.Tech (Pursuing)</p>
                                </div>
                            </li>
                            <li class="flex items-start gap-3">
                                <div class="w-8 h-8 rounded-lg bg-indigo-500/10 text-indigo-400 flex items-center justify-center shrink-0 mt-0.5">
                                    <i class="fa-solid fa-location-dot text-sm"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-gray-400">Address</p>
                                    <p class="text-sm font-semibold text-white">Teka Naka, Nari Road, Nagpur</p>
                                </div>
                            </li>
                            <li class="flex items-start gap-3">
                                <div class="w-8 h-8 rounded-lg bg-emerald-500/10 text-emerald-400 flex items-center justify-center shrink-0 mt-0.5">
                                    <i class="fa-solid fa-phone text-sm"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-gray-400">Phone</p>
                                    <p class="text-sm font-semibold text-white">+91 7499491802</p>
                                </div>
                            </li>
                        </ul>
                    </div>

                    <div class="pt-4 border-t border-gray-800">
                        <a href="https://www.linkedin.com/in/mayank-chandrakapure-3b8a68383" target="_blank" class="w-full py-2.5 px-4 rounded-xl bg-gray-800 hover:bg-gray-700 text-white font-medium text-sm flex items-center justify-center gap-2 transition-colors">
                            <i class="fa-brands fa-linkedin text-brand-400"></i> View LinkedIn Profile
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="education" class="py-20 relative bg-gray-900/40">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-semibold text-brand-400 tracking-widest uppercase mb-2">Academic Background</h2>
                <h3 class="font-heading text-3xl sm:text-4xl font-bold text-white">Education Details</h3>
                <div class="w-12 h-1 bg-brand-500 mx-auto rounded-full mt-4"></div>
            </div>

            <div class="max-w-4xl mx-auto space-y-8">
                <!-- Degree Card -->
                <div class="glass-card rounded-2xl p-6 sm:p-8 border border-gray-800 relative overflow-hidden group">
                    <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4 mb-4">
                        <div>
                            <span class="inline-block px-3 py-1 rounded-full bg-brand-500/10 text-brand-400 text-xs font-bold uppercase mb-2">Undergraduate Degree</span>
                            <h4 class="font-heading text-2xl font-bold text-white">Bachelor of Technology (B.Tech)</h4>
                        </div>
                        <span class="px-4 py-1.5 rounded-full bg-emerald-500/10 text-emerald-400 text-xs font-semibold border border-emerald-500/20">
                            Currently Pursuing
                        </span>
                    </div>
                    <p class="text-lg font-medium text-gray-200 mb-2">
                        <i class="fa-solid fa-building-columns text-brand-400 mr-2"></i>
                        S B Jain Institute of Technology, Research and Management
                    </p>
                    <p class="text-sm text-gray-400">
                        <i class="fa-solid fa-location-dot mr-1"></i> Nagpur, Maharashtra
                    </p>
                </div>

                <!-- HSC Card -->
                <div class="glass-card rounded-2xl p-6 sm:p-8 border border-gray-800 relative overflow-hidden group">
                    <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4 mb-4">
                        <div>
                            <span class="inline-block px-3 py-1 rounded-full bg-indigo-500/10 text-indigo-400 text-xs font-bold uppercase mb-2">Higher Secondary Certificate (HSC)</span>
                            <h4 class="font-heading text-2xl font-bold text-white">Senior Secondary Schooling</h4>
                        </div>
                        <span class="px-4 py-1.5 rounded-full bg-brand-500/10 text-brand-400 text-xs font-semibold border border-brand-500/20">
                            Score: 71%
                        </span>
                    </div>
                    <p class="text-lg font-medium text-gray-200 mb-2">
                        <i class="fa-solid fa-school text-indigo-400 mr-2"></i>
                        St. Paul College
                    </p>
                    <p class="text-sm text-gray-400">
                        <i class="fa-solid fa-location-dot mr-1"></i> Hudkeshwar, Nagpur, Maharashtra
                    </p>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="py-20 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-semibold text-brand-400 tracking-widest uppercase mb-2">Core Competencies</h2>
                <h3 class="font-heading text-3xl sm:text-4xl font-bold text-white">Skills & Focus Areas</h3>
                <div class="w-12 h-1 bg-brand-500 mx-auto rounded-full mt-4"></div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="glass-card rounded-2xl p-6 border border-gray-800 text-center hover:-translate-y-1 transition-transform duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-brand-500/10 text-brand-400 flex items-center justify-center text-2xl mx-auto mb-4">
                        <i class="fa-solid fa-microchip"></i>
                    </div>
                    <h4 class="font-heading text-lg font-bold text-white mb-2">Engineering Basics</h4>
                    <p class="text-xs text-gray-400">Structured analysis, system logic, and engineering fundamentals.</p>
                </div>

                <div class="glass-card rounded-2xl p-6 border border-gray-800 text-center hover:-translate-y-1 transition-transform duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-indigo-500/10 text-indigo-400 flex items-center justify-center text-2xl mx-auto mb-4">
                        <i class="fa-solid fa-code"></i>
                    </div>
                    <h4 class="font-heading text-lg font-bold text-white mb-2">Web Development</h4>
                    <p class="text-xs text-gray-400">Building user interfaces with HTML, CSS, JavaScript, and Tailwind.</p>
                </div>

                <div class="glass-card rounded-2xl p-6 border border-gray-800 text-center hover:-translate-y-1 transition-transform duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-purple-500/10 text-purple-400 flex items-center justify-center text-2xl mx-auto mb-4">
                        <i class="fa-solid fa-users"></i>
                    </div>
                    <h4 class="font-heading text-lg font-bold text-white mb-2">Teamwork</h4>
                    <p class="text-xs text-gray-400">Active participation in technical projects and collaborative study groups.</p>
                </div>

                <div class="glass-card rounded-2xl p-6 border border-gray-800 text-center hover:-translate-y-1 transition-transform duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-emerald-500/10 text-emerald-400 flex items-center justify-center text-2xl mx-auto mb-4">
                        <i class="fa-solid fa-lightbulb"></i>
                    </div>
                    <h4 class="font-heading text-lg font-bold text-white mb-2">Problem Solving</h4>
                    <p class="text-xs text-gray-400">Adaptable mindset focused on continuous learning and acquiring technical skills.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="py-20 relative bg-gray-900/40">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-semibold text-brand-400 tracking-widest uppercase mb-2">Get In Touch</h2>
                <h3 class="font-heading text-3xl sm:text-4xl font-bold text-white">Contact Information</h3>
                <div class="w-12 h-1 bg-brand-500 mx-auto rounded-full mt-4"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start max-w-6xl mx-auto">
                <div class="lg:col-span-5 space-y-6">
                    <div class="glass-card rounded-2xl p-6 sm:p-8 border border-gray-800 space-y-6">
                        <h4 class="font-heading text-xl font-bold text-white mb-2">Contact Details</h4>
                        
                        <!-- Phone -->
                        <div class="flex items-center gap-4">
                            <a href="tel:+917499491802" class="w-12 h-12 rounded-xl bg-brand-500/10 border border-brand-500/20 text-brand-400 flex items-center justify-center text-lg hover:bg-brand-500 hover:text-white transition-all duration-300">
                                <i class="fa-solid fa-phone"></i>
                            </a>
                            <div>
                                <p class="text-xs text-gray-400 font-medium">Call Me</p>
                                <p class="text-base font-semibold text-white">+91 7499491802</p>
                            </div>
                        </div>

                        <!-- LinkedIn -->
                        <div class="flex items-center gap-4">
                            <a href="https://www.linkedin.com/in/mayank-chandrakapure-3b8a68383" target="_blank" class="w-12 h-12 rounded-xl bg-indigo-500/10 border border-indigo-500/20 text-indigo-400 flex items-center justify-center text-lg hover:bg-indigo-500 hover:text-white transition-all duration-300">
                                <i class="fa-brands fa-linkedin"></i>
                            </a>
                            <div>
                                <p class="text-xs text-gray-400 font-medium">LinkedIn Profile</p>
                                <p class="text-base font-semibold text-white">Mayank Chandrakapure</p>
                            </div>
                        </div>

                        <!-- Address -->
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-xl bg-rose-500/10 border border-rose-500/20 text-rose-400 flex items-center justify-center text-lg">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <p class="text-xs text-gray-400 font-medium">Address</p>
                                <p class="text-base font-semibold text-white">At Nagpur, Teka Naka, Nari Road, Maharashtra</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-7">
                    <div class="glass-card rounded-2xl p-6 sm:p-8 border border-gray-800">
                        <h4 class="font-heading text-xl font-bold text-white mb-6">Send Me a Message</h4>
                        <form id="contact-form" class="space-y-4">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-semibold text-gray-300 mb-2">YOUR NAME</label>
                                    <input type="text" required placeholder="John Doe" class="w-full px-4 py-3 rounded-xl bg-gray-900/80 border border-gray-700 text-white placeholder-gray-500 focus:outline-none focus:border-brand-500 text-sm transition-colors">
                                </div>
                                <div>
                                    <label class="block text-xs font-semibold text-gray-300 mb-2">YOUR EMAIL</label>
                                    <input type="email" required placeholder="john@example.com" class="w-full px-4 py-3 rounded-xl bg-gray-900/80 border border-gray-700 text-white placeholder-gray-500 focus:outline-none focus:border-brand-500 text-sm transition-colors">
                                </div>
                            </div>
                            <div>
                                <label class="block text-xs font-semibold text-gray-300 mb-2">SUBJECT</label>
                                <input type="text" required placeholder="Inquiry / Message" class="w-full px-4 py-3 rounded-xl bg-gray-900/80 border border-gray-700 text-white placeholder-gray-500 focus:outline-none focus:border-brand-500 text-sm transition-colors">
                            </div>
                            <div>
                                <label class="block text-xs font-semibold text-gray-300 mb-2">MESSAGE</label>
                                <textarea rows="4" required placeholder="Write your message here..." class="w-full px-4 py-3 rounded-xl bg-gray-900/80 border border-gray-700 text-white placeholder-gray-500 focus:outline-none focus:border-brand-500 text-sm transition-colors resize-none"></textarea>
                            </div>

                            <button type="submit" class="w-full py-3.5 px-6 rounded-xl bg-gradient-to-r from-brand-500 to-indigo-600 hover:from-brand-600 hover:to-indigo-700 text-white font-semibold transition-all duration-300 shadow-lg shadow-brand-500/25">
                                Send Message
                            </button>
                        </form>
                        <div id="form-status" class="hidden mt-4 p-3 rounded-xl bg-emerald-500/20 text-emerald-400 text-sm text-center">
                            Thank you! Your message has been sent successfully.
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer class="py-8 border-t border-gray-800 bg-gray-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4">
            <p class="text-sm text-gray-400 text-center sm:text-left">
                © 2026 <span class="text-white font-semibold">Mayank Jagjiwan Chandrakapure</span>. All rights reserved.
            </p>
            <div class="flex items-center gap-4">
                <a href="https://www.linkedin.com/in/mayank-chandrakapure-3b8a68383" target="_blank" class="w-9 h-9 rounded-full bg-gray-800 text-gray-300 hover:bg-brand-500 hover:text-white flex items-center justify-center text-sm transition-colors">
                    <i class="fa-brands fa-linkedin"></i>
                </a>
                <a href="tel:+917499491802" class="w-9 h-9 rounded-full bg-gray-800 text-gray-300 hover:bg-brand-500 hover:text-white flex items-center justify-center text-sm transition-colors">
                    <i class="fa-solid fa-phone"></i>
                </a>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Navigation Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Navbar Scroll Styling
        window.addEventListener('scroll', () => {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 20) {
                navbar.classList.add('bg-gray-950/80', 'backdrop-blur-md', 'border-b', 'border-gray-800');
            } else {
                navbar.classList.remove('bg-gray-950/80', 'backdrop-blur-md', 'border-b', 'border-gray-800');
            }
        });

        // Form Submit Simulation
        const contactForm = document.getElementById('contact-form');
        const formStatus = document.getElementById('form-status');

        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            formStatus.classList.remove('hidden');
            contactForm.reset();
            setTimeout(() => {
                formStatus.classList.add('hidden');
            }, 5000);
        });
    </script>
</body>
</html>
