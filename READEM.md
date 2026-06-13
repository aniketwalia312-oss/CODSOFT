# CODSOFT
                                          LEVEL-1
My first task as a web developer intern in CODSOFT. and the task really help me in developing new skills and how to face challenges and make perfections at the same time,I enjoyed while working on my project and it was good fun. I would say... 

TASK-1:-(MY PORTFOLIO)

FILE:
      [index.html](https://github.com/user-attachments/files/28916201/index.html)

FOR MOBILE: https://nexusjobboard.netlify.app/

 CODE:<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aniket Walia | Premium Tech Portfolio</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;900&family=Fira+Code:wght@300;400;600&family=Outfit:wght@300;400;500;700;900&family=Space+Grotesk:wght@400;600;700;900&display=swap" rel="stylesheet">
    
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Outfit', 'sans-serif'],
                        display: ['Space Grotesk', 'sans-serif'],
                        logo: ['Cinzel', 'serif'],
                        mono: ['Fira Code', 'monospace'],
                    },
                    colors: {
                        dark: '#010103',
                        darker: '#000000',
                        accent: {
                            400: '#38bdf8',
                            500: '#00f2fe',
                            600: '#4facfe',
                            900: '#0c4a6e',
                        },
                        neon: {
                            pink: '#ff00ff',
                            purple: '#b026ff',
                        }
                    },
                    animation: {
                        'blob': 'blob 7s infinite',
                        'spin-slow': 'spin 12s linear infinite',
                        'float': 'float 6s ease-in-out infinite',
                        'glitch': 'glitch 1s linear infinite',
                    },
                    keyframes: {
                        blob: {
                            '0%': { transform: 'translate(0px, 0px) scale(1)' },
                            '33%': { transform: 'translate(30px, -50px) scale(1.1)' },
                            '66%': { transform: 'translate(-20px, 20px) scale(0.9)' },
                            '100%': { transform: 'translate(0px, 0px) scale(1)' },
                        },
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-20px)' },
                        }
                    }
                }
            }
        }
    </script>
    
    <style>
        :root {
            --cursor-x: 50%;
            --cursor-y: 50%;
        }

        body {
            background-color: #010103;
            color: #e2e8f0;
            overflow-x: hidden;
            cursor: none; 
        }
        
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #010103; }
        ::-webkit-scrollbar-thumb { background: #1e293b; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #00f2fe; }

        .cursor-glow {
            position: fixed; top: 0; left: 0; width: 400px; height: 400px;
            background: radial-gradient(circle, rgba(0, 242, 254, 0.1) 0%, transparent 70%);
            border-radius: 50%; transform: translate(-50%, -50%);
            pointer-events: none; z-index: 1; transition: opacity 0.3s;
        }
        .cursor-dot {
            position: fixed; top: 0; left: 0; width: 6px; height: 6px;
            background-color: #00f2fe; border-radius: 50%; transform: translate(-50%, -50%);
            pointer-events: none; z-index: 9999; box-shadow: 0 0 10px #00f2fe, 0 0 20px #00f2fe;
        }
        .cursor-ring {
            position: fixed; top: 0; left: 0; width: 36px; height: 36px;
            border: 1px solid rgba(0, 242, 254, 0.5); border-radius: 50%;
            transform: translate(-50%, -50%); pointer-events: none; z-index: 9998;
            transition: width 0.15s, height 0.15s, background-color 0.15s;
        }

        .glitch-wrapper { position: relative; display: inline-block; }
        .glitch-text {
            position: relative; font-weight: 900; color: white;
            text-shadow: 0 0 10px rgba(255,255,255,0.3);
        }
        .glitch-text::before, .glitch-text::after {
            content: attr(data-text); position: absolute; top: 0; left: 0;
            width: 100%; height: 100%; opacity: 0.8;
        }
        .glitch-text::before {
            left: 2px; text-shadow: -2px 0 #ff00ff;
            clip: rect(44px, 450px, 56px, 0); animation: glitch-anim 5s infinite linear alternate-reverse;
        }
        .glitch-text::after {
            left: -2px; text-shadow: -2px 0 #00f2fe;
            clip: rect(44px, 450px, 56px, 0); animation: glitch-anim2 5s infinite linear alternate-reverse;
        }
        @keyframes glitch-anim {
            0% { clip: rect(21px, 9999px, 86px, 0); }
            5% { clip: rect(98px, 9999px, 35px, 0); }
            10% { clip: rect(31px, 9999px, 5px, 0); }
            15% { clip: rect(10px, 9999px, 95px, 0); }
            20% { clip: rect(20px, 9999px, 20px, 0); }
            100% { clip: rect(20px, 9999px, 20px, 0); }
        }
        @keyframes glitch-anim2 {
            0% { clip: rect(15px, 9999px, 50px, 0); }
            5% { clip: rect(50px, 9999px, 10px, 0); }
            10% { clip: rect(80px, 9999px, 60px, 0); }
            15% { clip: rect(20px, 9999px, 90px, 0); }
            20% { clip: rect(0px, 9999px, 0px, 0); }
            100% { clip: rect(0px, 9999px, 0px, 0); }
        }

        .glass-card-hover {
            position: relative; background: rgba(15, 23, 42, 0.4);
            border: 1px solid rgba(255, 255, 255, 0.05); overflow: hidden;
            backdrop-filter: blur(12px); border-radius: 1.5rem; transition: transform 0.3s ease, border-color 0.3s ease;
        }
        .glass-card-hover::before {
            content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
            background: radial-gradient(800px circle at var(--mouse-x) var(--mouse-y), rgba(0, 242, 254, 0.06), transparent 40%);
            z-index: 0; pointer-events: none; transition: opacity 0.5s; opacity: 0;
        }
        .glass-card-hover:hover::before { opacity: 1; }
        .glass-card-hover:hover { border-color: rgba(0, 242, 254, 0.3); transform: translateY(-5px); }
        .glass-card-content { position: relative; z-index: 10; }

        .terminal-window {
            background: rgba(5, 5, 10, 0.8); border: 1px solid #1e293b;
            border-radius: 10px; overflow: hidden; box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }
        .terminal-header {
            background: #0f172a; padding: 8px 15px; display: flex; align-items: center; gap: 8px; border-bottom: 1px solid #1e293b;
        }
        .terminal-dot { width: 12px; height: 12px; border-radius: 50%; }
        
        .browser-mockup {
            border: 1px solid rgba(0, 242, 254, 0.2);
            border-radius: 12px; overflow: hidden; background: #000;
            box-shadow: 0 20px 50px rgba(0,0,0,0.5), 0 0 30px rgba(0, 242, 254, 0.05);
        }
        .browser-header {
            background: rgba(15, 23, 42, 0.9); border-bottom: 1px solid rgba(255,255,255,0.1);
            padding: 10px 15px; display: flex; align-items: center; gap: 10px;
        }

        .photo-frame {
            position: relative; border-radius: 20px; padding: 4px;
            background: linear-gradient(45deg, #00f2fe, #b026ff, #00f2fe);
            background-size: 300% 300%; animation: gradient-shift 4s ease infinite;
            box-shadow: 0 0 30px rgba(0, 242, 254, 0.3);
        }
        .photo-inner {
            border-radius: 16px; overflow: hidden; background: #010103; width: 100%; height: 100%;
        }
        @keyframes gradient-shift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .text-gradient {
            background: linear-gradient(to right, #00f2fe 0%, #4facfe 50%, #b026ff 100%);
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
            background-clip: text; background-size: 200% auto; animation: textShine 4s linear infinite;
        }
        @keyframes textShine { to { background-position: 200% center; } }

        .reveal { opacity: 0; transform: translateY(50px) scale(0.95); transition: all 1s cubic-bezier(0.5, 0, 0, 1); }
        .reveal.active { opacity: 1; transform: translateY(0) scale(1); }

        #particles-js { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: 0; pointer-events: none; }
        
        .nav-glass {
            background: rgba(1, 1, 3, 0.7); backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }
    </style>
</head>
<body class="antialiased font-sans selection:bg-accent-500 selection:text-dark">

    <div id="particles-js"></div>

    <div class="cursor-glow" id="cursor-glow"></div>
    <div class="cursor-dot" id="cursor-dot"></div>
    <div class="cursor-ring" id="cursor-ring"></div>

    <!-- Preloader -->
    <div id="preloader" class="fixed inset-0 bg-dark z-[99999] flex flex-col items-center justify-center transition-opacity duration-700">
        <div class="font-logo font-black text-4xl text-white tracking-[0.3em] mb-4 glitch-wrapper">
            <span class="glitch-text" data-text="A.W.">A.W.</span>
        </div>
        <div class="w-48 h-1 bg-gray-800 rounded-full overflow-hidden">
            <div class="h-full bg-gradient-to-r from-accent-400 to-neon-purple w-full origin-left animate-pulse"></div>
        </div>
        <div class="mt-4 font-mono text-xs text-accent-500 tracking-widest uppercase animate-pulse">Initializing System...</div>
    </div>

    <nav class="fixed w-full z-50 transition-all duration-300 py-4" id="navbar">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex items-center justify-between rounded-2xl px-6 py-3 transition-all duration-300" id="nav-inner">
                <!-- Unique Logo -->
                <a href="#" class="font-logo font-black text-2xl tracking-widest text-white group flex items-center gap-2">
                    <span class="text-accent-500 group-hover:text-white transition-colors duration-300">A</span>
                    <span class="text-white group-hover:text-neon-purple transition-colors duration-300">W</span>
                </a>

                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8 items-center bg-white/5 px-8 py-2.5 rounded-full border border-white/10 backdrop-blur-md">
                    <a href="#home" class="text-xs tracking-widest uppercase font-bold text-gray-400 hover:text-accent-500 transition-colors">Home</a>
                    <a href="#about" class="text-xs tracking-widest uppercase font-bold text-gray-400 hover:text-accent-500 transition-colors">About</a>
                    <a href="#skills" class="text-xs tracking-widest uppercase font-bold text-gray-400 hover:text-accent-500 transition-colors">Skills</a>
                    <a href="#projects" class="text-xs tracking-widest uppercase font-bold text-gray-400 hover:text-accent-500 transition-colors">Projects</a>
                    <a href="#resume" class="text-xs tracking-widest uppercase font-bold text-gray-400 hover:text-accent-500 transition-colors">Resume</a>
                </div>

                <!-- Hire Me Button -->
                <div class="hidden md:block">
                    <a href="#contact" class="px-6 py-2.5 text-sm font-bold text-dark bg-white rounded-full hover:shadow-[0_0_20px_rgba(255,255,255,0.4)] transition-all transform hover:scale-105 flex items-center gap-2">
                        <div class="w-2 h-2 rounded-full bg-green-500 animate-pulse"></div>
                        Hire Me
                    </a>
                </div>

                <!-- Mobile Menu Button -->
                <button class="md:hidden text-gray-300 hover:text-white focus:outline-none" id="mobile-menu-btn">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div class="md:hidden hidden absolute top-full left-0 w-full px-6 pb-4 transition-all" id="mobile-menu">
            <div class="bg-dark/95 backdrop-blur-xl rounded-2xl flex flex-col space-y-4 p-6 text-center border border-white/10 shadow-2xl">
                <a href="#home" class="text-lg font-medium text-gray-300">Home</a>
                <a href="#about" class="text-lg font-medium text-gray-300">About</a>
                <a href="#projects" class="text-lg font-medium text-gray-300">Projects</a>
                <a href="#resume" class="text-lg font-medium text-gray-300">Resume</a>
                <a href="#contact" class="text-lg font-bold text-accent-500 mt-4 border-t border-white/10 pt-4">Let's Talk</a>
            </div>
        </div>
    </nav>

    <section id="home" class="relative min-h-screen flex items-center justify-center pt-20 overflow-hidden">
        <!-- Animated Background Orbs -->
        <div class="absolute top-1/3 left-1/4 w-[30rem] h-[30rem] bg-accent-600 rounded-full mix-blend-screen filter blur-[150px] opacity-20 animate-blob"></div>
        <div class="absolute bottom-1/3 right-1/4 w-[30rem] h-[30rem] bg-neon-purple rounded-full mix-blend-screen filter blur-[150px] opacity-20 animate-blob" style="animation-delay: 2s;"></div>
        
        <div class="relative max-w-7xl mx-auto px-6 flex flex-col items-center text-center z-10 w-full mt-10">
            <!-- Tagline Badge -->
            <div class="reveal active inline-flex items-center gap-3 px-6 py-2 rounded-full border border-white/10 bg-white/5 backdrop-blur-md mb-8">
                <i class="fas fa-bolt text-accent-500"></i>
                <span class="text-xs font-bold tracking-[0.2em] uppercase text-gray-300">Transforming ideas into digital reality</span>
            </div>
            
            <!-- Glitch Name -->
            <div class="reveal active glitch-wrapper mb-6">
                <h1 class="glitch-text font-display text-5xl md:text-7xl lg:text-[8rem] font-black tracking-tighter leading-none uppercase" data-text="ANIKET WALIA">
                    ANIKET WALIA
                </h1>
            </div>
            
            <!-- Typing Subtitle -->
            <h2 class="reveal active h-8 text-xl md:text-3xl font-mono text-accent-400 mb-8 max-w-3xl">
                > <span id="typed-hero"></span><span class="animate-ping">_</span>
            </h2>
            
            <p class="reveal active text-base md:text-lg text-gray-400 max-w-2xl leading-relaxed mb-12 font-light">
                Hailing from Naraingarh, Haryana, pursuing B.Tech CSE from <span class="text-white font-medium border-b border-accent-500/50 pb-0.5">Maharishi Markandeshwar (Deemed to be University)</span>. I specialize in Full-Stack Architecture, Artificial Intelligence, and Algorithmic Solutions.
            </p>
            
            <div class="reveal active flex flex-col sm:flex-row gap-5">
                <a href="#projects" class="px-8 py-4 bg-white text-dark font-black tracking-widest uppercase text-sm rounded-full hover:shadow-[0_0_30px_rgba(255,255,255,0.4)] transition-all transform hover:scale-105 flex items-center justify-center gap-3">
                    View Projects <i class="fas fa-arrow-right"></i>
                </a>
                <a href="#contact" class="px-8 py-4 rounded-full bg-transparent text-white border border-white/20 font-bold uppercase tracking-widest text-sm hover:border-accent-500 hover:text-accent-400 transition-all flex items-center justify-center gap-3">
                    <i class="fab fa-github text-xl"></i> Let's Connect
                </a>
            </div>
        </div>

        <!-- Scroll Indicator -->
        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 flex flex-col items-center gap-3 animate-bounce opacity-60 hover:opacity-100 cursor-pointer" onclick="document.getElementById('about').scrollIntoView()">
            <span class="text-[10px] tracking-[0.3em] uppercase font-bold text-white">Scroll Down</span>
            <div class="w-[1px] h-12 bg-gradient-to-b from-white to-transparent"></div>
        </div>
    </section>

    <section id="about" class="py-32 relative z-10">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
                
                <!-- Left: Framed Photo -->
                <div class="reveal relative flex justify-center lg:justify-start">
                    <div class="relative w-full max-w-md aspect-[4/5] photo-frame animate-float">
                        <div class="photo-inner relative">
                            <!-- Overlay gradient to blend bottom of image into darkness -->
                            <div class="absolute inset-0 bg-gradient-to-t from-dark via-transparent to-transparent z-10 opacity-60"></div>
                            
                            <!-- EXACT USER IMAGE EMBEDDED HERE -->
                            <img src="./aniket%20walia.jpeg.jpeg" alt="Aniket Walia" 
                                 class="w-full h-full object-cover object-center filter contrast-125 saturate-110"
                                 onerror="this.src='https://placehold.co/800x1000/010103/00f2fe?text=Image+Not+Found'">
                        </div>
                        
                        <!-- Floating Badge -->
                        <div class="absolute -right-6 -bottom-6 bg-dark/80 backdrop-blur-md border border-white/10 rounded-2xl p-5 shadow-2xl z-20 flex items-center gap-4 hover:scale-110 transition-transform">
                            <div class="w-12 h-12 rounded-full bg-gradient-to-br from-accent-500 to-neon-purple flex items-center justify-center text-white text-xl shadow-[0_0_15px_rgba(0,242,254,0.5)]">
                                <i class="fas fa-code"></i>
                            </div>
                            <div>
                                <div class="text-xs font-bold tracking-widest uppercase text-gray-400">Status</div>
                                <div class="text-lg font-black text-white">Coding</div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Right: Terminal & Bio -->
                <div class="reveal">
                    <div class="inline-flex items-center gap-3 text-accent-500 font-bold tracking-[0.2em] uppercase text-sm mb-6">
                        <span class="w-12 h-[2px] bg-gradient-to-r from-accent-500 to-transparent"></span>
                        Profile Initialization
                    </div>
                    
                    <h2 class="text-4xl md:text-5xl lg:text-6xl font-display font-black text-white mb-8 leading-tight">
                        Engineer of <br/><span class="text-gradient">Digital Ecosystems.</span>
                    </h2>
                    
                    <!-- Terminal Window -->
                    <div class="terminal-window mb-8">
                        <div class="terminal-header">
                            <div class="terminal-dot bg-red-500"></div>
                            <div class="terminal-dot bg-yellow-500"></div>
                            <div class="terminal-dot bg-green-500"></div>
                            <div class="ml-4 text-xs font-mono text-gray-500">aniket@portfolio:~</div>
                        </div>
                        <div class="p-5 font-mono text-sm leading-relaxed text-gray-300">
                            <p class="mb-2"><span class="text-green-400">aniket@portfolio:~$</span> whoami</p>
                            <p class="text-accent-400 mb-4">> Aniket Walia. Software Developer & AI Enthusiast.</p>
                            
                            <p class="mb-2"><span class="text-green-400">aniket@portfolio:~$</span> cat passion.txt</p>
                            <p class="text-gray-400 mb-4">> Forward-thinking Computer Science student with a specialized focus on emerging AI technologies and modern software development pipelines. Proven track record in rapid prototyping and technical leadership through national hackathons.</p>
                            
                            <p><span class="text-green-400">aniket@portfolio:~$</span> <span class="animate-pulse">_</span></p>
                        </div>
                    </div>

                    <div class="grid grid-cols-2 gap-6 border-t border-white/10 pt-8">
                        <div>
                            <div class="text-3xl font-black text-white mb-1">AI / MERN</div>
                            <div class="text-xs font-bold tracking-widest uppercase text-accent-600">Core Focus</div>
                        </div>
                        <div>
                            <div class="text-3xl font-black text-white mb-1">CI/CD</div>
                            <div class="text-xs font-bold tracking-widest uppercase text-neon-purple">Deployment</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="py-32 relative z-10 bg-darker/50 border-y border-white/5">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center max-w-3xl mx-auto mb-20 reveal">
                <h2 class="text-4xl md:text-5xl font-display font-black text-white mb-4">Technical <span class="text-gradient">Arsenal</span></h2>
                <p class="text-gray-400 font-light">The technologies, frameworks, and methodologies I leverage to engineer solutions.</p>
            </div>

            <!-- CSS Grid for Cards with mouse tracking -->
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6 cards-container">
                
                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center">
                    <div class="glass-card-content">
                        <i class="fas fa-brain text-5xl text-[#00f2fe] mb-2 drop-shadow-[0_0_15px_rgba(0,242,254,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">AI Integration</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">OpenAI, Gemini</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 50ms;">
                    <div class="glass-card-content">
                        <i class="fab fa-react text-5xl text-[#61DAFB] mb-2 animate-[spin_10s_linear_infinite] drop-shadow-[0_0_15px_rgba(97,218,251,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">React / Frontend</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">UI Architecture</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 100ms;">
                    <div class="glass-card-content">
                        <i class="fab fa-node-js text-5xl text-[#339933] mb-2 drop-shadow-[0_0_15px_rgba(51,153,51,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Node.js</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">Backend Services</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 150ms;">
                    <div class="glass-card-content">
                        <i class="fas fa-database text-5xl text-[#4facfe] mb-2 drop-shadow-[0_0_15px_rgba(79,172,254,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Databases</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">Data Structures</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 200ms;">
                    <div class="glass-card-content">
                        <i class="fas fa-server text-5xl text-[#b026ff] mb-2 drop-shadow-[0_0_15px_rgba(176,38,255,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Vercel</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">CI/CD Deploy</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 250ms;">
                    <div class="glass-card-content">
                        <i class="fas fa-code-branch text-5xl text-[#A8B9CC] mb-2 drop-shadow-[0_0_15px_rgba(168,185,204,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Algorithms</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">Core Concepts</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 300ms;">
                    <div class="glass-card-content">
                        <i class="fab fa-git-alt text-5xl text-[#F05032] mb-2 drop-shadow-[0_0_15px_rgba(240,80,50,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Version Control</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">Git, GitHub</p>
                    </div>
                </div>

                <div class="glass-card-hover p-8 flex flex-col items-center justify-center gap-5 reveal text-center" style="transition-delay: 350ms;">
                    <div class="glass-card-content">
                        <i class="fas fa-cogs text-5xl text-[#E34F26] mb-2 drop-shadow-[0_0_15px_rgba(227,79,38,0.4)]"></i>
                        <h3 class="font-bold text-white tracking-wider">Software Eng.</h3>
                        <p class="text-xs text-gray-500 font-mono mt-2">Architecture</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="py-32 relative z-10">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-end mb-16 reveal">
                <div>
                    <div class="inline-flex items-center gap-3 text-accent-500 font-bold tracking-[0.2em] uppercase text-sm mb-4">
                        <span class="w-12 h-[2px] bg-gradient-to-r from-accent-500 to-transparent"></span>
                        Showcase
                    </div>
                    <h2 class="text-4xl md:text-5xl lg:text-6xl font-display font-black text-white">Live <span class="text-gradient">Deployments</span></h2>
                </div>
            </div>

            <!-- Feature Project: RapidCR -->
            <div class="glass-card-hover rounded-3xl overflow-hidden reveal mb-20 border border-accent-500/30">
                <div class="glass-card-content p-0">
                    <div class="grid grid-cols-1 lg:grid-cols-12">
                        <!-- Project Info Left -->
                        <div class="lg:col-span-4 p-10 flex flex-col justify-center bg-dark/80 border-r border-white/5">
                            <div class="flex items-center gap-3 mb-6">
                                <span class="px-3 py-1 text-[10px] font-black bg-red-500 text-white rounded-full tracking-widest uppercase animate-pulse">Google Solution Challenge '26</span>
                            </div>
                            <h3 class="text-3xl font-display font-black text-white mb-4">RapidCR Platform</h3>
                            <p class="text-gray-400 mb-8 text-sm leading-relaxed font-light">
                                Engineered core components for the RapidCR platform alongside Team Quantyx. A unified command, communication, and citizen-safety platform designed to coordinate responders during disasters. 
                            </p>
                            
                            <div class="flex flex-wrap gap-2 mb-8">
                                <span class="px-3 py-1 text-xs font-mono rounded bg-white/5 border border-white/10 text-accent-400">Web App</span>
                                <span class="px-3 py-1 text-xs font-mono rounded bg-white/5 border border-white/10 text-accent-400">Deployment</span>
                                <span class="px-3 py-1 text-xs font-mono rounded bg-white/5 border border-white/10 text-accent-400">System Design</span>
                            </div>
                            
                            <div class="mt-auto">
                                <p class="text-xs text-gray-500 font-mono mb-2 flex items-center gap-2"><i class="fas fa-hand-pointer text-accent-500"></i> Interact with the live application on the right.</p>
                            </div>
                        </div>

                        <!-- Embedded Website Right -->
                        <div class="lg:col-span-8 bg-black relative">
                            <div class="browser-mockup border-none rounded-none h-full w-full">
                                <div class="browser-header">
                                    <div class="flex gap-2">
                                        <div class="w-3 h-3 rounded-full bg-red-500/80"></div>
                                        <div class="w-3 h-3 rounded-full bg-yellow-500/80"></div>
                                        <div class="w-3 h-3 rounded-full bg-green-500/80"></div>
                                    </div>
                                    <div class="w-full bg-white/10 rounded px-3 py-1 text-center font-mono text-[10px] text-gray-400 truncate flex items-center justify-center gap-2">
                                    <i class="fas fa-lock text-green-400"></i> https://rapidcr.aniketwalia.dev
                                </div>
                            </div>
                            
                            <!-- EXACT HTML PROJECT EMBEDDED HERE with explicit relative pathing -->
                            <iframe src="./rapidemer.html" class="w-full h-[500px] lg:h-[600px] border-none bg-dark" title="RapidCR Live Application" sandbox="allow-scripts allow-same-origin allow-popups allow-forms"></iframe>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Smart India Hackathon Project -->
            <div class="glass-card-hover rounded-2xl reveal w-full max-w-4xl mx-auto">
                <div class="glass-card-content p-8 flex flex-col md:flex-row items-center gap-8">
                    <div class="w-full md:w-1/3 flex justify-center">
                        <div class="w-32 h-32 rounded-full border border-white/10 flex items-center justify-center relative">
                            <div class="absolute inset-0 bg-neon-purple/20 rounded-full blur-xl"></div>
                            <i class="fas fa-users-cog text-5xl text-white relative z-10"></i>
                        </div>
                    </div>
                    <div class="w-full md:w-2/3">
                        <h3 class="text-2xl font-display font-black text-white mb-2">Smart India Hackathon (SIH) '25</h3>
                        <h4 class="text-accent-500 font-mono text-sm mb-3">Team Leader | Team THE OUTLIERS</h4>
                        <p class="text-gray-400 mb-4 text-sm leading-relaxed">
                            Spearheaded a dynamic team of developers to prototype and present a robust software solution under a strict timeframe. Orchestrated project architecture and timeline management, ensuring timely milestone completion utilizing GitHub for strict version control.
                        </p>
                        <a href="https://github.com/aniketwalia312-oss" target="_blank" class="inline-flex items-center gap-2 text-xs font-bold uppercase tracking-widest text-accent-500 hover:text-white transition-colors">
                            View GitHub <i class="fab fa-github text-lg"></i>
                        </a>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <section id="resume" class="py-32 relative z-10 bg-darker border-y border-white/5">
        <div class="absolute inset-0 bg-[url('https://www.transparenttextures.com/patterns/cubes.png')] opacity-[0.03] mix-blend-screen pointer-events-none"></div>
        <div class="max-w-6xl mx-auto px-6 reveal">
            
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-display font-black text-white mb-4">Official <span class="text-gradient">Documentation</span></h2>
                <p class="text-gray-400 font-light max-w-2xl mx-auto">Review my complete professional profile, academic achievements, and technical expertise directly below.</p>
            </div>

            <!-- PDF Resume Embed Window -->
            <div class="browser-mockup relative mx-auto shadow-[0_0_50px_rgba(176,38,255,0.15)] transition-all hover:shadow-[0_0_80px_rgba(176,38,255,0.3)]">
                <div class="browser-header justify-between">
                    <div class="flex items-center gap-4">
                        <div class="flex gap-2">
                            <div class="w-3 h-3 rounded-full bg-red-500"></div>
                            <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                            <div class="w-3 h-3 rounded-full bg-green-500"></div>
                        </div>
                        <div class="text-xs font-mono text-gray-300 flex items-center gap-2">
                            <i class="fas fa-file-pdf text-accent-400"></i> Aniket_Walia_Visual_Resume_v2.pdf
                        </div>
                    </div>
                    <!-- Updated button to link directly to the new PDF resume page -->
                    <a href="./Aniket_Walia_Visual_Resume_v2.pdf" target="_blank" class="bg-white text-dark hover:bg-accent-500 transition-colors px-4 py-1.5 rounded text-xs font-bold uppercase tracking-widest flex items-center gap-2">
                        <i class="fas fa-external-link-alt"></i> Open Fullscreen
                    </a>
                </div>
                
                <div class="w-full h-[600px] md:h-[800px] bg-[#010103] relative">
                    <!-- PDF Resume File Embedded directly here -->
                    <iframe src="./Aniket_Walia_Visual_Resume_v2.pdf" class="w-full h-full border-none" title="Aniket Walia PDF Resume"></iframe>
                </div>
            </div>

        </div>
    </section>

    <section id="contact" class="py-32 relative z-10">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
                
                <!-- Contact Info Left -->
                <div class="reveal">
                    <h2 class="text-5xl md:text-6xl font-display font-black text-white mb-6">Initiate <br><span class="text-gradient">Handshake.</span></h2>
                    <p class="text-gray-400 mb-12 text-lg font-light leading-relaxed">
                        Whether you have a question, a project proposal, or just want to talk code, my inbox is always open. 
                    </p>
                    
                    <div class="space-y-6">
                        <!-- Direct Links -->
                        <a href="mailto:aniket.walia@email.com" class="glass-card-hover p-6 flex items-center gap-6 group rounded-2xl block">
                            <div class="glass-card-content flex items-center gap-6 w-full">
                                <div class="w-14 h-14 rounded-full bg-white/5 flex items-center justify-center text-accent-500 text-2xl group-hover:bg-accent-500 group-hover:text-dark transition-colors border border-white/10">
                                    <i class="fas fa-envelope"></i>
                                </div>
                                <div>
                                    <div class="text-xs font-mono text-gray-500 mb-1">EMAIL</div>
                                    <div class="text-white font-bold text-lg">aniket.walia@email.com</div>
                                </div>
                            </div>
                        </a>
                        
                        <a href="tel:+917900000809" class="glass-card-hover p-6 flex items-center gap-6 group rounded-2xl block">
                            <div class="glass-card-content flex items-center gap-6 w-full">
                                <div class="w-14 h-14 rounded-full bg-white/5 flex items-center justify-center text-neon-purple text-2xl group-hover:bg-neon-purple group-hover:text-white transition-colors border border-white/10">
                                    <i class="fas fa-phone-alt"></i>
                                </div>
                                <div>
                                    <div class="text-xs font-mono text-gray-500 mb-1">PHONE</div>
                                    <div class="text-white font-bold text-lg">+91 7900000809</div>
                                </div>
                            </div>
                        </a>
                    </div>
                    
                    <div class="mt-12 flex gap-4">
                        <a href="https://www.linkedin.com/in/aniket-walia-2b2a4737a?utm_source=share_via&utm_content=profile&utm_medium=member_android" target="_blank" class="w-12 h-12 rounded-full border border-white/20 flex items-center justify-center text-white hover:bg-[#0A66C2] hover:border-[#0A66C2] transition-all hover:-translate-y-1">
                            <i class="fab fa-linkedin-in text-xl"></i>
                        </a>
                        <a href="https://github.com/aniketwalia312-oss" target="_blank" class="w-12 h-12 rounded-full border border-white/20 flex items-center justify-center text-white hover:bg-white hover:text-dark hover:border-white transition-all hover:-translate-y-1">
                            <i class="fab fa-github text-xl"></i>
                        </a>
                    </div>
                </div>

                <!-- Form Right -->
                <div class="reveal">
                    <form onsubmit="event.preventDefault(); document.getElementById('success-msg').style.display='block'; this.reset();" class="glass-card-hover p-10 rounded-3xl h-full flex flex-col justify-center">
                        <div class="glass-card-content space-y-6">
                            <div class="mb-4">
                                <div class="text-xs font-mono text-accent-500 mb-2">> SECURE_MESSAGE_PROTOCOL</div>
                                <div class="w-full h-[1px] bg-gradient-to-r from-accent-500/50 to-transparent"></div>
                            </div>

                            <div>
                                <input type="text" required class="w-full bg-black/50 border border-white/10 rounded-lg px-5 py-4 text-white placeholder-gray-600 focus:outline-none focus:border-accent-500 focus:ring-1 focus:ring-accent-500 transition-all font-mono text-sm" placeholder="NAME / ALIAS">
                            </div>
                            <div>
                                <input type="email" required class="w-full bg-black/50 border border-white/10 rounded-lg px-5 py-4 text-white placeholder-gray-600 focus:outline-none focus:border-accent-500 focus:ring-1 focus:ring-accent-500 transition-all font-mono text-sm" placeholder="EMAIL_ADDRESS">
                            </div>
                            <div>
                                <textarea required rows="4" class="w-full bg-black/50 border border-white/10 rounded-lg px-5 py-4 text-white placeholder-gray-600 focus:outline-none focus:border-accent-500 focus:ring-1 focus:ring-accent-500 transition-all font-mono text-sm resize-none" placeholder="ENTER_PAYLOAD..."></textarea>
                            </div>
                            <button type="submit" class="w-full py-4 bg-white text-dark font-black tracking-widest uppercase rounded-lg hover:shadow-[0_0_20px_rgba(255,255,255,0.3)] transition-all transform hover:scale-[1.02] flex justify-center items-center gap-3">
                                TRANSMIT <i class="fas fa-paper-plane"></i>
                            </button>
                            
                            <div id="success-msg" class="hidden text-green-400 font-mono text-xs text-center mt-4 border border-green-500/30 bg-green-500/10 py-3 rounded">
                                > [OK] Payload delivered successfully.
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <footer class="py-8 border-t border-white/10 bg-black text-center relative z-10">
        <div class="max-w-7xl mx-auto px-6 flex flex-col md:flex-row justify-between items-center gap-4">
            <p class="font-mono text-xs text-gray-500">© 2026 ANIKET WALIA. SYS_ONLINE.</p>
            <div class="flex items-center gap-2">
                <span class="w-2 h-2 rounded-full bg-green-500 animate-pulse"></span>
                <span class="font-mono text-xs text-gray-500">NARAINGARH · AMBALA</span>
            </div>
        </div>
    </footer>

    <!-- Scripts -->
    <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
    
    <script>
        // Preloader
        window.addEventListener('load', () => {
            setTimeout(() => {
                const preloader = document.getElementById('preloader');
                preloader.style.opacity = '0';
                setTimeout(() => preloader.style.display = 'none', 700);
            }, 1000); 
        });

        // Mouse Tracking
        const cursorDot = document.getElementById('cursor-dot');
        const cursorRing = document.getElementById('cursor-ring');
        const cursorGlow = document.getElementById('cursor-glow');
        const glassCards = document.querySelectorAll('.glass-card-hover');

        window.addEventListener('mousemove', (e) => {
            const x = e.clientX;
            const y = e.clientY;
            
            cursorDot.style.left = `${x}px`;
            cursorDot.style.top = `${y}px`;
            
            cursorRing.animate({ left: `${x}px`, top: `${y}px` }, { duration: 150, fill: "forwards" });
            cursorGlow.animate({ left: `${x}px`, top: `${y}px` }, { duration: 300, fill: "forwards" });

            glassCards.forEach(card => {
                const rect = card.getBoundingClientRect();
                const cardX = x - rect.left;
                const cardY = y - rect.top;
                card.style.setProperty('--mouse-x', `${cardX}px`);
                card.style.setProperty('--mouse-y', `${cardY}px`);
            });
        });

        document.querySelectorAll('a, button, input, textarea, iframe').forEach(el => {
            el.addEventListener('mouseenter', () => {
                cursorRing.style.width = '50px';
                cursorRing.style.height = '50px';
                cursorRing.style.borderColor = '#ff00ff';
                cursorRing.style.backgroundColor = 'rgba(255,0,255,0.1)';
            });
            el.addEventListener('mouseleave', () => {
                cursorRing.style.width = '36px';
                cursorRing.style.height = '36px';
                cursorRing.style.borderColor = 'rgba(0, 242, 254, 0.5)';
                cursorRing.style.backgroundColor = 'transparent';
            });
        });

        // Hacker Typing Effect
        const heroTypedTarget = document.getElementById('typed-hero');
        const phrases = ["BUILDING DIGITAL ARCHITECTURES", "SOLVING COMPLEX PROBLEMS", "WRITING ELEGANT CODE"];
        let phraseIndex = 0;
        let charIndex = 0;
        let isDeleting = false;

        function typeWriter() {
            const currentPhrase = phrases[phraseIndex];
            
            if (isDeleting) {
                heroTypedTarget.innerText = currentPhrase.substring(0, charIndex - 1);
                charIndex--;
            } else {
                heroTypedTarget.innerText = currentPhrase.substring(0, charIndex + 1);
                charIndex++;
            }

            let typeSpeed = isDeleting ? 30 : 70;

            if (!isDeleting && charIndex === currentPhrase.length) {
                typeSpeed = 2000;
                isDeleting = true;
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                phraseIndex = (phraseIndex + 1) % phrases.length;
                typeSpeed = 500;
            }

            setTimeout(typeWriter, typeSpeed);
        }
        setTimeout(typeWriter, 1500);

        // 3D Particles
        particlesJS('particles-js', {
            "particles": {
                "number": { "value": 40, "density": { "enable": true, "value_area": 1000 } },
                "color": { "value": ["#00f2fe", "#b026ff", "#ffffff"] },
                "shape": { "type": "circle" },
                "opacity": { "value": 0.4, "random": true, "anim": { "enable": true, "speed": 1, "opacity_min": 0.1, "sync": false } },
                "size": { "value": 3, "random": true },
                "line_linked": { "enable": true, "distance": 150, "color": "#00f2fe", "opacity": 0.1, "width": 1 },
                "move": { "enable": true, "speed": 1, "direction": "none", "random": true, "straight": false, "out_mode": "out", "bounce": false }
            },
            "interactivity": {
                "detect_on": "canvas",
                "events": {
                    "onhover": { "enable": true, "mode": "grab" },
                    "onclick": { "enable": true, "mode": "push" },
                    "resize": true
                }
            },
            "retina_detect": true
        });

        // Navbar Styling on Scroll
        window.addEventListener('scroll', () => {
            const nav = document.getElementById('navbar');
            const navInner = document.getElementById('nav-inner');
            if (window.scrollY > 50) {
                navInner.classList.add('nav-glass');
                nav.classList.remove('py-4');
                nav.classList.add('py-2');
            } else {
                navInner.classList.remove('nav-glass');
                nav.classList.remove('py-2');
                nav.classList.add('py-4');
            }
        });

        // Mobile Menu
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => mobileMenu.classList.add('hidden'));
        });

        // Reveal Animation
        const observerOptions = { root: null, rootMargin: '0px', threshold: 0.1 };
        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                    observer.unobserve(entry.target); 
                }
            });
        }, observerOptions);

        document.querySelectorAll('.reveal').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
 
