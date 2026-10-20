<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Delmy Lopez | Creative & Data Specialist</title>
  
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            burgundy: {
              950: '#0E0406',
              900: '#1B090E',
              800: '#2C1118',
              700: '#431924',
            },
            rose: {
              gold: '#E3C1B4',
              soft: '#FAF3F0',
              accent: '#C59A8B'
            }
          },
          fontFamily: {
            serif: ['Cormorant Garamond', 'Georgia', 'serif'],
            sans: ['Inter', 'sans-serif'],
          }
        }
      }
    }
  </script>

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>

  <style>
    body {
      background-color: #0E0406;
      color: #FAF3F0;
      font-family: 'Inter', sans-serif;
      overflow-x: hidden;
    }

    .font-serif {
      font-family: 'Cormorant Garamond', Georgia, serif;
    }

    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 6px;
    }
    ::-webkit-scrollbar-track {
      background: #0E0406;
    }
    ::-webkit-scrollbar-thumb {
      background: #2C1118;
      border-radius: 3px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #C59A8B;
    }

    /* Arch frame decoration */
    .arch-frame {
      border-top-left-radius: 180px;
      border-top-right-radius: 180px;
    }

    .rose-gradient-border {
      background: linear-gradient(135deg, #E3C1B4 0%, #431924 50%, #C59A8B 100%);
      padding: 1px;
    }

    /* Glassmorphism subtle effect */
    .glass-card {
      background: rgba(27, 9, 14, 0.6);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(227, 193, 180, 0.12);
    }

    .glass-card:hover {
      border-color: rgba(227, 193, 180, 0.35);
    }
  </style>
</head>
<body class="antialiased selection:bg-rose-gold selection:text-burgundy-950">

  <!-- NAVIGATION -->
  <header class="fixed top-0 left-0 right-0 z-50 bg-burgundy-950/80 backdrop-blur-md border-b border-rose-gold/10 transition-all duration-300">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <!-- LOGO: Replaced AM Studio with Delmy Lopez -->
      <a href="#" class="font-serif text-2xl tracking-wider text-rose-soft font-light hover:text-rose-gold transition-colors flex items-center gap-2">
        <span class="inline-block w-2 h-2 rounded-full bg-rose-gold"></span>
        DELMY LOPEZ
      </a>

      <!-- Desktop Nav -->
      <nav class="hidden md:flex items-center space-x-8 text-xs uppercase tracking-widest text-rose-soft/70">
        <a href="#about" class="hover:text-rose-gold transition-colors">About</a>
        <a href="#education" class="hover:text-rose-gold transition-colors">Education</a>
        <a href="#experience" class="hover:text-rose-gold transition-colors">Experience</a>
        <a href="#certifications" class="hover:text-rose-gold transition-colors">Certifications</a>
        <a href="#skills" class="hover:text-rose-gold transition-colors">Skills</a>
        <a href="#contact" class="hover:text-rose-gold transition-colors">Contact</a>
      </nav>

      <!-- Contact CTA -->
      <a href="mailto:marylenalopez.d@gmail.com" class="hidden sm:inline-flex items-center text-xs uppercase tracking-widest px-4 py-2 rounded-full border border-rose-gold/30 text-rose-gold hover:bg-rose-gold hover:text-burgundy-950 transition-all duration-300">
        Get in Touch
      </a>

      <!-- Mobile menu button -->
      <button id="menu-btn" class="md:hidden text-rose-soft focus:outline-none">
        <i data-lucide="menu" class="w-6 h-6"></i>
      </button>
    </div>

    <!-- Mobile Nav Menu -->
    <div id="mobile-menu" class="hidden md:hidden bg-burgundy-900 border-b border-rose-gold/10 px-6 py-4 flex flex-col space-y-4 text-xs uppercase tracking-widest text-rose-soft/80">
      <a href="#about" class="hover:text-rose-gold py-1">About</a>
      <a href="#education" class="hover:text-rose-gold py-1">Education</a>
      <a href="#experience" class="hover:text-rose-gold py-1">Experience</a>
      <a href="#certifications" class="hover:text-rose-gold py-1">Certifications</a>
      <a href="#skills" class="hover:text-rose-gold py-1">Skills</a>
      <a href="#contact" class="hover:text-rose-gold py-1">Contact</a>
    </div>
  </header>

  <!-- HERO SECTION -->
  <section id="about" class="min-h-screen pt-28 pb-16 flex items-center justify-center relative overflow-hidden">
    <!-- Subtle Background Ambient Light -->
    <div class="absolute top-1/4 -left-32 w-96 h-96 bg-burgundy-700/20 rounded-full blur-3xl pointer-events-none"></div>
    <div class="absolute bottom-10 right-0 w-96 h-96 bg-rose-accent/10 rounded-full blur-3xl pointer-events-none"></div>

    <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-12 gap-12 items-center">
      
      <!-- Text Intro -->
      <div class="md:col-span-7 space-y-6 text-center md:text-left order-2 md:order-1">
        <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-burgundy-800/80 border border-rose-gold/20 text-xs tracking-widest text-rose-gold uppercase">
          <i data-lucide="sparkles" class="w-3.5 h-3.5"></i>
          <span>Data Analyst, Web Page Design & Content Creator</span>
        </div>

        <h1 class="font-serif text-4xl sm:text-6xl lg:text-7xl font-light leading-tight tracking-tight text-rose-soft">
          Precision in Data.<br/>
          <span class="italic font-normal text-rose-gold">Elegance</span> in Web & Content.
        </h1>

        <p class="text-rose-soft/70 text-base sm:text-lg max-w-xl font-light leading-relaxed">
          Hello, I'm <strong class="text-rose-soft font-normal">Delmy Lopez</strong>. I specialize in critical legal document verification, CRM data processing, high attention-to-detail analysis, creative digital marketing strategy, and Web Design.
        </p>

        <!-- Key Metrics / Stats -->
        <div class="grid grid-cols-3 gap-4 pt-4 border-t border-rose-gold/10">
          <div>
            <span class="block font-serif text-2xl sm:text-3xl text-rose-gold">100%</span>
            <span class="text-xs text-rose-soft/60 uppercase tracking-wider">Accuracy</span>
          </div>
          <div>
            <span class="block font-serif text-2xl sm:text-3xl text-rose-gold">3+ Yrs</span>
            <span class="text-xs text-rose-soft/60 uppercase tracking-wider">Experience</span>
          </div>
          <div>
            <span class="block font-serif text-2xl sm:text-3xl text-rose-gold">7+</span>
            <span class="text-xs text-rose-soft/60 uppercase tracking-wider">Certificates</span>
          </div>
        </div>

        <div class="pt-4 flex flex-wrap gap-4 justify-center md:justify-start">
          <a href="#experience" class="px-6 py-3 rounded-full bg-rose-gold text-burgundy-950 font-medium text-xs uppercase tracking-widest hover:bg-rose-soft transition-all duration-300 shadow-lg shadow-rose-gold/10">
            View Experience
          </a>
          <button onclick="openAiPitchModal()" class="px-6 py-3 rounded-full border border-rose-gold/40 text-rose-gold text-xs uppercase tracking-widest hover:bg-rose-gold/10 transition-all duration-300 flex items-center gap-2">
            <i data-lucide="sparkles" class="w-4 h-4 text-rose-gold"></i>
            <span>Tailor Pitch (AI)</span>
          </button>
        </div>
      </div>

      <!-- PORTRAIT IMAGE WITH ARCH STYLING -->
      <div class="md:col-span-5 flex justify-center order-1 md:order-2">
        <div class="relative group max-w-xs sm:max-w-sm w-full">
          <!-- Background Glow Frame -->
          <div class="absolute -inset-1 rounded-[180px] bg-gradient-to-b from-rose-gold/40 via-burgundy-700/30 to-rose-accent/20 blur-lg opacity-70 group-hover:opacity-100 transition duration-500"></div>
          
          <!-- Outer Decorative Border Arch -->
          <div class="relative p-2 rounded-t-[180px] rounded-b-3xl border border-rose-gold/30 bg-burgundy-900/80 shadow-2xl overflow-hidden">
            <div class="arch-frame overflow-hidden bg-burgundy-950 aspect-[4/5] relative">
              <img 
                src="watermarked_img_17634668984190486336.jpg" 
                alt="Delmy Lopez Professional Portrait" 
                class="w-full h-full object-cover object-center transition-transform duration-700 group-hover:scale-105"
                onerror="this.src='https://placehold.co/400x500/1B090E/E3C1B4?text=Delmy+Lopez'"
              />
              <div class="absolute inset-0 bg-gradient-to-t from-burgundy-950/80 via-transparent to-transparent"></div>
            </div>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- EDUCATION SECTION -->
  <section id="education" class="py-20 bg-burgundy-900/60 border-t border-rose-gold/10 relative">
    <div class="max-w-7xl mx-auto px-6">
      
      <!-- Section Header -->
      <div class="text-center max-w-2xl mx-auto mb-16">
        <h2 class="text-xs uppercase tracking-widest text-rose-gold mb-2">Academic Background</h2>
        <h3 class="font-serif text-3xl sm:text-5xl text-rose-soft font-light">Higher Education</h3>
        <div class="w-12 h-0.5 bg-rose-gold mx-auto mt-4"></div>
      </div>

      <div class="glass-card rounded-2xl p-8 max-w-4xl mx-auto">
        <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-rose-gold/10 pb-6 mb-6 gap-4">
          <div>
            <span class="text-xs text-rose-gold font-medium uppercase tracking-widest">Currently Enrolled • 1st Year, 2nd Semester</span>
            <h4 class="font-serif text-3xl sm:text-4xl text-rose-soft mt-1">Licenciatura en Mercadotecnia (Marketing)</h4>
            <p class="text-sm text-rose-soft/70 mt-2 flex items-center gap-1.5 font-light">
              <i data-lucide="graduation-cap" class="w-4 h-4 text-rose-gold"></i>
              <span>Universidad Mariano Gálvez de Guatemala</span>
            </p>
          </div>
          <div class="px-4 py-2 rounded-full bg-burgundy-800 border border-rose-gold/30 text-rose-gold text-xs tracking-wider uppercase font-medium whitespace-nowrap">
            In Progress
          </div>
        </div>

        <h5 class="text-xs uppercase tracking-widest text-rose-gold mb-4 font-medium flex items-center gap-2">
          <i data-lucide="book-open" class="w-4 h-4"></i> Current Semester Coursework (Pensum)
        </h5>

        <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-4">
          <!-- Course 1 -->
          <div class="p-5 rounded-xl bg-burgundy-950/60 border border-rose-gold/15 flex items-center">
            <h6 class="text-sm font-medium text-rose-soft">Lenguaje e Investigación Documental</h6>
          </div>

          <!-- Course 2 -->
          <div class="p-5 rounded-xl bg-burgundy-950/60 border border-rose-gold/15 flex items-center">
            <h6 class="text-sm font-medium text-rose-soft">Matemática Aplicada II</h6>
          </div>

          <!-- Course 3 -->
          <div class="p-5 rounded-xl bg-burgundy-950/60 border border-rose-gold/15 flex items-center">
            <h6 class="text-sm font-medium text-rose-soft">Administración de Negocios II</h6>
          </div>

          <!-- Course 4 -->
          <div class="p-5 rounded-xl bg-burgundy-950/60 border border-rose-gold/15 flex items-center">
            <h6 class="text-sm font-medium text-rose-soft">Legislación Mercantil</h6>
          </div>

          <!-- Course 5 -->
          <div class="p-5 rounded-xl bg-burgundy-950/60 border border-rose-gold/15 sm:col-span-2 lg:col-span-2 flex items-center">
            <h6 class="text-sm font-medium text-rose-soft">Psicología del Consumidor</h6>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- WORK EXPERIENCE SECTION -->
  <section id="experience" class="py-20 bg-burgundy-900/40 relative">
    <div class="max-w-7xl mx-auto px-6">
      
      <!-- Section Header -->
      <div class="text-center max-w-2xl mx-auto mb-16">
        <h2 class="text-xs uppercase tracking-widest text-rose-gold mb-2">Professional Career</h2>
        <h3 class="font-serif text-3xl sm:text-5xl text-rose-soft font-light">Work Experience</h3>
        <div class="w-12 h-0.5 bg-rose-gold mx-auto mt-4"></div>
      </div>

      <div class="grid md:grid-cols-2 gap-8">

        <!-- Icon (Lawsuit & CRM Analyst) -->
        <div class="glass-card rounded-2xl p-8 transition-all duration-300 relative group">
          <div class="flex justify-between items-start mb-4">
            <div>
              <span class="text-xs text-rose-gold font-medium uppercase tracking-widest">Current Role</span>
              <h4 class="font-serif text-2xl text-rose-soft mt-1">Icon</h4>
            </div>
            <div class="w-10 h-10 rounded-full bg-burgundy-800 border border-rose-gold/20 flex items-center justify-center text-rose-gold">
              <i data-lucide="scale" class="w-5 h-5"></i>
            </div>
          </div>
          <h5 class="text-sm text-rose-soft/80 font-medium mb-3">Legal Lawsuit Document & CRM Quality Analyst</h5>
          <ul class="text-sm text-rose-soft/70 space-y-2.5 font-light">
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Review and audit legal lawsuit documentation containing high-priority sensitive information.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Demonstrate rigorous attention to detail to ensure 100% compliance and error-free legal records.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Process, organize, and extract key case data into client CRM management systems seamlessly.</span>
            </li>
          </ul>
        </div>

        <!-- Conduent -->
        <div class="glass-card rounded-2xl p-8 transition-all duration-300 relative group">
          <div class="flex justify-between items-start mb-4">
            <div>
              <span class="text-xs text-rose-soft/50 font-medium uppercase tracking-widest">Dec 2024 - May 2025</span>
              <h4 class="font-serif text-2xl text-rose-soft mt-1">Conduent</h4>
            </div>
            <div class="w-10 h-10 rounded-full bg-burgundy-800 border border-rose-gold/20 flex items-center justify-center text-rose-gold">
              <i data-lucide="file-check-2" class="w-5 h-5"></i>
            </div>
          </div>
          <h5 class="text-sm text-rose-soft/80 font-medium mb-3">Back Office Specialist</h5>
          <ul class="text-sm text-rose-soft/70 space-y-2.5 font-light">
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Reviewed and verified complex documentation to align with strict internal procedures and client standards.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Handled sensitive data with high discretion adhering to strict international data privacy protocols.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Coordinated efficiently across cross-functional teams and client communication channels.</span>
            </li>
          </ul>
        </div>

        <!-- Telus International -->
        <div class="glass-card rounded-2xl p-8 transition-all duration-300 relative group">
          <div class="flex justify-between items-start mb-4">
            <div>
              <span class="text-xs text-rose-soft/50 font-medium uppercase tracking-widest">Aug 2023 - Dec 2024</span>
              <h4 class="font-serif text-2xl text-rose-soft mt-1">TELUS International</h4>
            </div>
            <div class="w-10 h-10 rounded-full bg-burgundy-800 border border-rose-gold/20 flex items-center justify-center text-rose-gold">
              <i data-lucide="users" class="w-5 h-5"></i>
            </div>
          </div>
          <h5 class="text-sm text-rose-soft/80 font-medium mb-3">Customer Care & Trainer Team Member</h5>
          <ul class="text-sm text-rose-soft/70 space-y-2.5 font-light">
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Assisted international client accounts, delivering detailed product insights and resolving complex inquiries.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Selected to join the Trainers Team to onboard and mentor new account representatives.</span>
            </li>
          </ul>
        </div>

        <!-- MIDES -->
        <div class="glass-card rounded-2xl p-8 transition-all duration-300 relative group">
          <div class="flex justify-between items-start mb-4">
            <div>
              <span class="text-xs text-rose-soft/50 font-medium uppercase tracking-widest">Feb 2022 - Jun 2022</span>
              <h4 class="font-serif text-2xl text-rose-soft mt-1">Ministerio de Desarrollo Social</h4>
            </div>
            <div class="w-10 h-10 rounded-full bg-burgundy-800 border border-rose-gold/20 flex items-center justify-center text-rose-gold">
              <i data-lucide="building-2" class="w-5 h-5"></i>
            </div>
          </div>
          <h5 class="text-sm text-rose-soft/80 font-medium mb-3">Administrative Assistant</h5>
          <ul class="text-sm text-rose-soft/70 space-y-2.5 font-light">
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Supported social welfare management in San Antonio La Paz with document processing in Word & Excel.</span>
            </li>
            <li class="flex items-start gap-2">
              <i data-lucide="check" class="w-4 h-4 text-rose-gold shrink-0 mt-0.5"></i>
              <span>Managed public beneficiary registry input in official government database systems.</span>
            </li>
          </ul>
        </div>

      </div>

    </div>
  </section>

  <!-- CERTIFICATIONS SECTION (PLATZI & INTECAP) -->
  <section id="certifications" class="py-20 relative">
    <div class="max-w-7xl mx-auto px-6">
      
      <div class="text-center max-w-2xl mx-auto mb-16">
        <h2 class="text-xs uppercase tracking-widest text-rose-gold mb-2">Continuous Learning</h2>
        <h3 class="font-serif text-3xl sm:text-5xl text-rose-soft font-light">Certifications & Diplomas</h3>
        <p class="text-rose-soft/60 text-sm mt-3 font-light">Verified coursework from Platzi and INTECAP</p>
        <div class="w-12 h-0.5 bg-rose-gold mx-auto mt-4"></div>
      </div>

      <!-- Certification Grid -->
      <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">

        <!-- Platzi Item 1 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2026</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Programación Básica</h4>
            <p class="text-xs text-rose-soft/60 font-light">16 hours theory & practice. Fundamental coding logic & structure.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 2 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2026</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Lovable Web Creation</h4>
            <p class="text-xs text-rose-soft/60 font-light">10 hours theory & practice. No-code web development and platform design.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 3 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2022</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Marca Personal</h4>
            <p class="text-xs text-rose-soft/60 font-light">11 hours. Personal branding strategy, storytelling & audience engagement.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 4 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2022</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Audioglosario de Contenido</h4>
            <p class="text-xs text-rose-soft/60 font-light">3 hours. Marketing content strategy and digital audio concepts.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 5 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2022</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Fotografía con Celular</h4>
            <p class="text-xs text-rose-soft/60 font-light">17 hours. Mobile visual composition, framing, photo editing & aesthetic lighting.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 6 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2022</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Marketing Digital</h4>
            <p class="text-xs text-rose-soft/60 font-light">17 hours. Digital ad campaigns, brand positioning & funnel optimization.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- Platzi Item 7 -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">PLATZI</span>
              <span>2020</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">English Writing</h4>
            <p class="text-xs text-rose-soft/60 font-light">7 hours. Intermediate business English grammar, structure & professional email syntax.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Verified ID</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

        <!-- INTECAP -->
        <div class="glass-card rounded-xl p-6 flex flex-col justify-between hover:-translate-y-1 transition-transform duration-300 border-rose-gold/30">
          <div>
            <div class="flex items-center justify-between text-xs text-rose-gold mb-3">
              <span class="font-mono">INTECAP</span>
              <span>Scholarship</span>
            </div>
            <h4 class="font-serif text-xl text-rose-soft mb-2">Finishing School</h4>
            <p class="text-xs text-rose-soft/60 font-light">Intensive English language immersion and global business communication training.</p>
          </div>
          <div class="mt-4 pt-3 border-t border-rose-gold/10 flex items-center justify-between text-[11px] text-rose-gold">
            <span>Scholarship Award</span>
            <i data-lucide="award" class="w-4 h-4"></i>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- SKILLS & LANGUAGES -->
  <section id="skills" class="py-20 bg-burgundy-900/40 border-t border-b border-rose-gold/10">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-12 gap-12 items-center">
      
      <div class="lg:col-span-5 space-y-6">
        <h2 class="text-xs uppercase tracking-widest text-rose-gold">Core Competencies</h2>
        <h3 class="font-serif text-3xl sm:text-5xl text-rose-soft font-light">Skills & Languages</h3>
        <p class="text-rose-soft/70 text-sm font-light leading-relaxed">
          Combining procedural precision for legal document processing with creative marketing and visual communication capabilities.
        </p>

        <!-- Languages -->
        <div class="space-y-4 pt-4">
          <h4 class="text-xs uppercase tracking-widest text-rose-gold">Language Proficiency</h4>
          
          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-rose-soft">Spanish</span>
              <span class="text-rose-gold">Native / Fluent</span>
            </div>
            <div class="w-full bg-burgundy-800 h-1.5 rounded-full overflow-hidden">
              <div class="bg-rose-gold h-full w-full"></div>
            </div>
          </div>

          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-rose-soft">English</span>
              <span class="text-rose-gold">C1 Advanced / Professional</span>
            </div>
            <div class="w-full bg-burgundy-800 h-1.5 rounded-full overflow-hidden">
              <div class="bg-rose-gold h-full w-[90%]"></div>
            </div>
          </div>

          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-rose-soft">Portuguese</span>
              <span class="text-rose-gold">Beginner</span>
            </div>
            <div class="w-full bg-burgundy-800 h-1.5 rounded-full overflow-hidden">
              <div class="bg-rose-gold h-full w-[30%]"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- Skill Pills -->
      <div class="lg:col-span-7 grid grid-cols-2 sm:grid-cols-3 gap-4">
        
        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="layout" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">Web Page Design</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">UX/UI & Layouts</p>
        </div>

        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="shield-check" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">Attention to Detail</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">Lawsuit verification</p>
        </div>

        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="database" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">CRM Processing</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">Client management</p>
        </div>

        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="lock" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">Data Privacy</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">Confidential handling</p>
        </div>

        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="camera" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">Mobile Photography</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">Visual curation</p>
        </div>

        <div class="glass-card p-5 rounded-xl text-center">
          <i data-lucide="globe-2" class="w-6 h-6 text-rose-gold mx-auto mb-2"></i>
          <h5 class="text-xs uppercase tracking-wider text-rose-soft font-medium">English C1</h5>
          <p class="text-[11px] text-rose-soft/50 mt-1">Fluent Communication</p>
        </div>

      </div>

    </div>
  </section>

  <!-- CONTACT SECTION -->
  <section id="contact" class="py-24 relative overflow-hidden">
    <div class="max-w-4xl mx-auto px-6 text-center relative z-10">
      
      <span class="text-xs uppercase tracking-widest text-rose-gold">Let's Connect</span>
      <h2 class="font-serif text-4xl sm:text-6xl text-rose-soft font-light mt-2 mb-6">Start a Conversation</h2>
      <p class="text-rose-soft/70 text-sm sm:text-base max-w-lg mx-auto font-light leading-relaxed mb-10">
        Whether you have a query regarding legal data auditing, CRM management, or creative projects, feel free to reach out.
      </p>

      <div class="flex flex-col sm:flex-row items-center justify-center gap-6">
        <!-- Email CTA -->
        <a href="mailto:marylenalopez.d@gmail.com" class="w-full sm:w-auto px-8 py-4 rounded-full bg-rose-gold text-burgundy-950 font-medium text-xs uppercase tracking-widest hover:bg-rose-soft transition-all duration-300 flex items-center justify-center gap-2 shadow-xl shadow-rose-gold/10">
          <i data-lucide="mail" class="w-4 h-4"></i>
          <span>marylenalopez.d@gmail.com</span>
        </a>

        <!-- Phone CTA -->
        <a href="tel:+50246042084" class="w-full sm:w-auto px-8 py-4 rounded-full border border-rose-gold/30 text-rose-soft font-medium text-xs uppercase tracking-widest hover:bg-burgundy-800 transition-all duration-300 flex items-center justify-center gap-2">
          <i data-lucide="phone" class="w-4 h-4 text-rose-gold"></i>
          <span>+502 4604 2084</span>
        </a>
      </div>

      <div class="mt-12 text-xs text-rose-soft/50 font-light flex items-center justify-center gap-2">
        <i data-lucide="map-pin" class="w-3.5 h-3.5 text-rose-gold"></i>
        <span>Guatemala City, Guatemala</span>
      </div>

    </div>
  </section>

  <!-- FOOTER -->
  <footer class="py-8 border-t border-rose-gold/10 text-center text-xs text-rose-soft/40">
    <div class="max-w-7xl mx-auto px-6 flex flex-col sm:flex-row justify-between items-center gap-4">
      <p class="font-serif text-sm text-rose-soft/70">Delmy Lopez</p>
      <p>© 2026 Delmy Marylena López López. All rights reserved.</p>
      <a href="https://platzi.com/@delmylopez/" target="_blank" class="hover:text-rose-gold transition-colors flex items-center gap-1">
        <span>Platzi Profile</span>
        <i data-lucide="external-link" class="w-3 h-3"></i>
      </a>
    </div>
  </footer>

  <div id="ai-pitch-modal" class="fixed inset-0 z-50 bg-burgundy-950/80 backdrop-blur-md hidden flex items-center justify-center p-4">
    <div class="bg-burgundy-900 border border-rose-gold/30 rounded-2xl max-w-lg w-full p-6 shadow-2xl relative">
      <button onclick="closeAiPitchModal()" class="absolute top-4 right-4 text-rose-soft/60 hover:text-rose-soft">
        <i data-lucide="x" class="w-5 h-5"></i>
      </button>

      <div class="flex items-center gap-2 mb-4">
        <i data-lucide="sparkles" class="w-5 h-5 text-rose-gold"></i>
        <h3 class="font-serif text-2xl text-rose-soft">Tailor Delmy's Proposal</h3>
      </div>
      <p class="text-xs text-rose-soft/70 mb-4 font-light">
        Generate a personalized introduction or project pitch tailored to your industry using Gemini AI.
      </p>

      <div class="space-y-4">
        <div>
          <label class="block text-xs uppercase tracking-wider text-rose-gold mb-1">Target Industry / Needs</label>
          <input id="pitch-industry" type="text" placeholder="e.g. Corporate Law Firm, E-commerce Web Redesign, CRM Data Audit" class="w-full bg-burgundy-950 border border-rose-gold/20 rounded-xl px-3 py-2 text-xs text-rose-soft focus:outline-none focus:border-rose-gold">
        </div>

        <button onclick="generateCustomPitch()" id="generate-pitch-btn" class="w-full py-2.5 rounded-full bg-rose-gold text-burgundy-950 text-xs uppercase tracking-widest font-medium hover:bg-rose-soft transition-all flex items-center justify-center gap-2">
          <i data-lucide="wand-2" class="w-4 h-4"></i>
          <span>Generate Custom Pitch</span>
        </button>

        <div id="pitch-result-container" class="hidden bg-burgundy-950/80 border border-rose-gold/20 rounded-xl p-4 mt-2">
          <span class="text-[10px] uppercase tracking-widest text-rose-gold block mb-1">Tailored Response</span>
          <p id="pitch-result-text" class="text-xs text-rose-soft/90 leading-relaxed font-light"></p>
        </div>
      </div>
    </div>
  </div>

  <!-- Lucide Icon Initialization & Mobile Menu Toggle Script -->
  <script>
    lucide.createIcons();

    // Mobile menu toggle logic
    const menuBtn = document.getElementById('menu-btn');
    const mobileMenu = document.getElementById('mobile-menu');

    if (menuBtn && mobileMenu) {
      menuBtn.addEventListener('click', () => {
        mobileMenu.classList.toggle('hidden');
      });

      // Close mobile menu on link click
      mobileMenu.querySelectorAll('a').forEach(link => {
        link.addEventListener('click', () => {
          mobileMenu.classList.add('hidden');
        });
      });
    }

    async function callGeminiApi(prompt, systemInstruction = "") {
      const apiKey = ""; // Canvas handles key runtime injection
      const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent?key=${apiKey}`;

      const payload = {
        contents: [{ parts: [{ text: prompt }] }]
      };

      if (systemInstruction) {
        payload.systemInstruction = { parts: [{ text: systemInstruction }] };
      }

      const response = await fetch(apiUrl, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(payload)
      });

      if (!response.ok) {
        throw new Error(`API error ${response.status}`);
      }

      const data = await response.json();
      return data.candidates?.[0]?.content?.parts?.[0]?.text || "No response received.";
    }

    // AI Pitch Customizer Modal Logic
    function openAiPitchModal() {
      document.getElementById('ai-pitch-modal').classList.remove('hidden');
    }

    function closeAiPitchModal() {
      document.getElementById('ai-pitch-modal').classList.add('hidden');
    }

    async function generateCustomPitch() {
      const industryInput = document.getElementById('pitch-industry').value.trim();
      const btn = document.getElementById('generate-pitch-btn');
      const resultContainer = document.getElementById('pitch-result-container');
      const resultText = document.getElementById('pitch-result-text');

      if (!industryInput) {
        alert("Please enter a target industry or need.");
        return;
      }

      btn.disabled = true;
      btn.innerHTML = `<i data-lucide="loader-2" class="w-4 h-4 animate-spin"></i> Generating Pitch...`;
      lucide.createIcons();

      const systemPrompt = "You are a professional luxury portfolio assistant for Delmy Lopez (Legal Lawsuit & CRM Data Analyst, Web Page Designer, Content Creator with C1 English). Write a concise, 2-3 sentence personalized pitch explaining how Delmy's skills directly solve problems for the specified target client/industry. Maintain an elegant, professional tone.";
      
      try {
        const pitch = await callGeminiApi(`Generate pitch for: ${industryInput}`, systemPrompt);
        resultText.innerText = pitch;
        resultContainer.classList.remove('hidden');
      } catch (err) {
        resultText.innerText = "Error generating pitch. Please try again.";
        resultContainer.classList.remove('hidden');
      } finally {
        btn.disabled = false;
        btn.innerHTML = `<i data-lucide="wand-2" class="w-4 h-4"></i> Generate Custom Pitch`;
        lucide.createIcons();
      }
    }
  </script>

</body>
</html>
