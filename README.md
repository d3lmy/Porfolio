<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Delmy Lopez | Creative &amp; Data Specialist</title>
<meta name="description" content="Delmy Lopez — analista de datos y documentos legales, diseñadora web y creadora de contenido en Guatemala.">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,400&family=Inter:wght@300;400;500;600&display=swap">
<style>
  :root { 
    --radius: .625rem; 
    --burgundy-950: oklch(13% .02 10); 
    --burgundy-900: oklch(17% .03 5); 
    --burgundy-800: oklch(22% .045 5); 
    --burgundy-700: oklch(29% .065 5); 
    --rose-gold: oklch(84% .045 40); 
    --rose-soft: oklch(97% .01 40); 
    --rose-accent: oklch(71% .06 35); 
    --background: var(--burgundy-950); 
    --foreground: var(--rose-soft); 
    --card: var(--burgundy-900); 
    --card-foreground: var(--rose-soft); 
    --primary: var(--rose-gold); 
    --primary-foreground: var(--burgundy-950); 
    --secondary: var(--burgundy-800); 
    --muted: var(--burgundy-800); 
    --muted-foreground: oklch(97% .01 40 / .65); 
    --accent: var(--burgundy-700); 
    --border: oklch(84% .045 40 / .12); 
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body { background-color: var(--background); color: var(--foreground); font-family: "Inter", sans-serif; -webkit-font-smoothing: antialiased; overflow-x: hidden; line-height: 1.5; }
  
  ::selection { background: var(--rose-gold); color: var(--burgundy-950); }
  
  /* Estilos generales y componentes */
  header { position: fixed; inset-x: 0; top: 0; z-index: 50; border-bottom: 1px solid var(--border); background-color: color-mix(in oklab, var(--burgundy-950) 80%, transparent); backdrop-filter: blur(12px); }
  .nav-container { max-width: 80rem; margin: 0 auto; display: flex; items-align: center; justify-content: space-between; padding: 1rem 1.5rem; align-items: center; }
  .logo { display: flex; align-items: center; gap: 0.5rem; font-family: "Cormorant Garamond", Georgia, serif; font-size: 1.5rem; font-weight: 300; letter-spacing: 0.05em; color: var(--rose-soft); text-decoration: none; }
  .logo span { display: inline-block; height: 0.5rem; width: 0.5rem; border-radius: 9999px; background-color: var(--rose-gold); }
  
  nav.desktop-nav { display: none; gap: 2rem; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--muted-foreground); }
  nav.desktop-nav a { color: inherit; text-decoration: none; transition: color 0.2s; }
  nav.desktop-nav a:hover { color: var(--rose-gold); }
  
  .btn-touch { display: none; border-radius: 9999px; border: 1px solid color-mix(in oklab, var(--rose-gold) 30%, transparent); padding: 0.5rem 1rem; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--rose-gold); text-decoration: none; transition: all 0.2s; }
  .btn-touch:hover { background-color: var(--rose-gold); color: var(--burgundy-950); }

  section { min-height: 100vh; display: flex; align-items: center; justify-content: center; position: relative; padding: 7rem 1.5rem 4rem 1.5rem; }
  .max-w-7xl { max-width: 80rem; margin: 0 auto; width: 100%; }

  /* Hero Section */
  .hero-grid { display: grid; gap: 3rem; align-items: center; grid-template-columns: 1fr; }
  .hero-content { display: flex; flex-direction: column; gap: 1.5rem; text-align: center; }
  .badge { display: inline-flex; align-items: center; gap: 0.5rem; border-radius: 9999px; border: 1px solid color-mix(in oklab, var(--rose-gold) 20%, transparent); background-color: color-mix(in oklab, var(--burgundy-800) 80%, transparent); padding: 0.25rem 0.75rem; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--rose-gold); width: fit-content; margin: 0 auto; }
  h1 { font-family: "Cormorant Garamond", Georgia, serif; font-size: 2.5rem; font-weight: 300; line-height: 1.2; letter-spacing: -0.025em; color: var(--rose-soft); }
  h1 span { font-style: italic; font-weight: 400; color: var(--rose-gold); }
  .hero-desc { max-width: 36rem; font-size: 1rem; font-weight: 300; line-height: 1.625; color: var(--muted-foreground); margin: 0 auto; }
  
  .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; border-top: 1px solid var(--border); padding-top: 1rem; }
  .stat-item span:first-child { display: block; font-family: "Cormorant Garamond", Georgia, serif; font-size: 1.5rem; color: var(--rose-gold); }
  .stat-item span:last-child { font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.05em; color: var(--muted-foreground); }

  .hero-buttons { display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; padding-top: 1rem; }
  .btn-primary { border-radius: 9999px; background-color: var(--rose-gold); padding: 0.75rem 1.5rem; font-size: 0.75rem; font-weight: 500; text-transform: uppercase; letter-spacing: 0.1em; color: var(--burgundy-950); text-decoration: none; box-shadow: 0 10px 15px -3px color-mix(in oklab, var(--rose-gold) 10%, transparent); transition: background-color 0.2s; }
  .btn-primary:hover { background-color: var(--rose-soft); }
  .btn-secondary { border-radius: 9999px; border: 1px solid color-mix(in oklab, var(--rose-gold) 40%, transparent); padding: 0.75rem 1.5rem; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--rose-gold); text-decoration: none; transition: background-color 0.2s; }
  .btn-secondary:hover { background-color: color-mix(in oklab, var(--rose-gold) 10%, transparent); }

  /* Secciones adicionales generadas */
  .section-title { font-family: "Cormorant Garamond", Georgia, serif; font-size: 2.25rem; font-weight: 300; color: var(--rose-soft); margin-bottom: 2rem; text-align: center; }
  .content-box { background-color: var(--card); border: 1px solid var(--border); border-radius: 1rem; padding: 2rem; margin-bottom: 1.5rem; }
  .content-box h3 { font-size: 1.25rem; color: var(--rose-gold); margin-bottom: 0.5rem; font-weight: 500; }
  .content-box p { color: var(--muted-foreground); font-size: 0.95rem; }

  /* Media Queries */
  @media(min-width: 768px) {
    nav.desktop-nav { display: flex; }
    .btn-touch { display: inline-flex; }
    .hero-grid { grid-template-columns: repeat(12, 1fr); gap: 3rem; }
    .hero-content { grid-span: span 7; grid-column: span 7; text-align: left; }
    .hero-content .badge, .hero-content .hero-buttons { margin: 0; justify-content: flex-start; }
    .hero-desc { margin: 0; }
    .hero-image-container { grid-column: span 5; display: flex; justify-content: center; }
  }
</style>
</head>
<body>

  <!-- Barra de Navegación -->
  <header>
    <div class="nav-container">
      <a href="#" class="logo">
        <span></span> DELMY LOPEZ
      </a>
      <nav class="desktop-nav">
        <a href="#about">Sobre mí</a>
        <a href="#education">Educación</a>
        <a href="#experience">Experiencia</a>
        <a href="#certifications">Certificaciones</a>
        <a href="#skills">Habilidades</a>
        <a href="#contact">Contacto</a>
      </nav>
      <a href="mailto:marylenalopez.d@gmail.com" class="btn-touch">Contactar</a>
    </div>
  </header>

  <!-- Sección Principal / Hero -->
  <section id="about">
    <div class="max-t-7xl max-w-7xl">
      <div class="hero-grid">
        <div class="hero-content">
          <div class="badge">
            Data Analyst, Web Page Design &amp; Content Creator
          </div>
          <h1>DESIGN<br><span>con</span> INTENTO</h1>
          <p class="hero-desc">
            Hola, soy <strong>Delmy Lopez</strong>. Me especializo en la verificación crítica de documentos legales, procesamiento de datos CRM, análisis detallado, estrategia de marketing digital y diseño web.
          </p>
          <div class="stats-grid">
            <div class="stat-item">
              <span>100%</span>
              <span>Precisión</span>
            </div>
            <div class="stat-item">
              <span>3+ Años</span>
              <span>Experiencia</span>
            </div>
            <div class="stat-item">
              <span>7+</span>
              <span>Certificados</span>
            </div>
          </div>
          <div class="hero-buttons">
            <a href="#experience" class="btn-primary">Ver Experiencia</a>
            <a href="#contact" class="btn-secondary">Contacto</a>
          </div>
        </div>
        <div class="hero-image-container" style="display: flex; justify-content: center; align-items: center;">
          <!-- Contenedor visual estético acorde al diseño original con bordes redondeados y tonos borgoña -->
          <div style="width: 260px; height: 320px; background: linear-gradient(to bottom, var(--burgundy-800), var(--burgundy-900)); border: 1.5px solid color-mix(in oklab, var(--rose-gold) 30%, transparent); border-top-left-radius: 150px; border-top-right-radius: 150px; border-bottom-left-radius: 1.5rem; border-bottom-right-radius: 1.5rem; display: flex; align-items: center; justify-content: center; box-shadow: 0 25px 50px -12px rgba(0,0,0,0.4);">
            <span style="font-family: 'Cormorant Garamond', serif; font-size: 5rem; color: var(--rose-gold); font-weight: 300;">DL</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Sección de Educación -->
  <section id="education" style="min-height: auto; padding: 5rem 1.5rem;">
    <div class="max-w-7xl">
      <h2 class="section-title">Educación</h2>
      <div class="content-box">
        <h3>Universidad Mariano Gálvez de Guatemala</h3>
        <p>Estudiante de primer año en el campus central (Zona 2), enfocada en disciplinas administrativas, económicas y del entorno digital.</p>
      </div>
    </div>
  </section>

  <!-- Sección de Experiencia -->
  <section id="experience" style="min-height: auto; padding: 5rem 1.5rem;">
    <div class="max-w-7xl">
      <h2 class="section-title">Experiencia Profesional</h2>
      <div class="content-box">
        <h3>Especialista en Datos y Verificación Documental</h3>
        <p>Enfoque riguroso en el análisis de documentos legales, procesamiento eficiente en CRM y garantía de calidad con alta atención al detalle.</p>
      </div>
      <div class="content-box">
        <h3>Diseño Web &amp; Creación de Contenido</h3>
        <p>Desarrollo de interfaces web funcionales, estilizadas y propuestas de marketing digital orientadas a resultados comerciales y de marca.</p>
      </div>
    </div>
  </section>

  <!-- Sección de Certificaciones y Habilidades -->
  <section id="skills" style="min-height: auto; padding: 5rem 1.5rem;">
    <div class="max-w-7xl">
      <h2 class="section-title">Habilidades y Certificaciones</h2>
      <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem;">
        <div class="content-box" style="margin-bottom: 0;">
          <h3>Análisis de Datos</h3>
          <p>Manejo de sistemas CRM, procesamiento avanzado y verificación de bases de datos con precisión milimétrica.</p>
        </div>
        <div class="content-box" style="margin-bottom: 0;">
          <h3>Diseño &amp; Multimedia</h3>
          <p>Creación de sitios web personalizados, optimización visual y estrategias de contenido creativo.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Sección de Contacto -->
  <section id="contact" style="padding: 5rem 1.5rem 6rem 1.5rem;">
    <div class="max-w-7xl" style="text-align: center;">
      <h2 class="section-title">¿Trabajamos Juntos?</h2>
      <p style="color: var(--muted-foreground); margin-bottom: 2rem; max-width: 30rem; margin-left: auto; margin-right: auto;">
        Siempre estoy abierta a nuevos proyectos, consultas profesionales o colaboraciones creativas. ¡Escríbeme!
      </p>
      <a href="mailto:marylenalopez.d@gmail.com" class="btn-primary">Enviar un Correo</a>
    </div>
  </section>

</body>
</html>
