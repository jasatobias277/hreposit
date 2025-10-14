<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portafolio del Proyecto | Jairo Salcedo</title>
  <style>
    /* --- RESET --- */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #333;
      background-color: #f7f8fa;
    }

    /* --- NAVBAR --- */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #0056b3;
      color: white;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      display: flex;
      list-style: none;
      gap: 1.5rem;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      transition: 0.3s;
    }

    .nav-links a:hover {
      color: #d1e7ff;
    }

    .menu-toggle {
      display: none;
      font-size: 1.8rem;
      cursor: pointer;
    }

    /* --- HERO --- */
    .hero {
      background: linear-gradient(rgba(0, 86, 179, 0.7), rgba(0, 86, 179, 0.7)), url('https://picsum.photos/1600/800?grayscale');
      background-size: cover;
      background-position: center;
      text-align: center;
      color: white;
      padding: 8rem 2rem;
    }

    .hero h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.1rem;
      max-width: 700px;
      margin: 0 auto 1.5rem;
    }

    .btn {
      background: white;
      color: #0056b3;
      padding: 0.7rem 1.5rem;
      border-radius: 5px;
      font-weight: bold;
      text-decoration: none;
      transition: 0.3s;
    }

    .btn:hover {
      background: #e5e5e5;
    }

    /* --- SECCIONES --- */
    .section {
      padding: 4rem 2rem;
      text-align: center;
    }

    .bg-light {
      background: #eef1f7;
    }

    .section h3 {
      color: #0056b3;
      font-size: 2rem;
      margin-bottom: 1.5rem;
    }

    /* --- TECNOLOGÍAS --- */
    .tech-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .tech-card {
      background: white;
      border-radius: 10px;
      padding: 1rem;
      box-shadow: 0 3px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .tech-card:hover {
      transform: scale(1.05);
    }

    .tech-card img {
      height: 60px;
    }

    /* --- GALERÍA --- */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }

    .gallery img {
      width: 100%;
      border-radius: 10px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    /* --- FORMULARIO --- */
    .contact-form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 500px;
      margin: 0 auto;
    }

    .contact-form input,
    .contact-form textarea {
      padding: 0.8rem;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1rem;
    }

    .contact-form textarea {
      resize: vertical;
      height: 120px;
    }

    /* --- FOOTER --- */
    footer {
      background: #0056b3;
      color: white;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
    }

    /* --- RESPONSIVE --- */
    @media (max-width: 768px) {
      .nav-links {
        display: none;
        flex-direction: column;
        background: #004a99;
        position: absolute;
        top: 60px;
        right: 0;
        width: 200px;
        padding: 1rem;
      }

      .nav-links.show {
        display: flex;
      }

      .menu-toggle {
        display: block;
      }
    }
  </style>
</head>
<body>

  <!-- NAVBAR -->
  <header>
    <nav class="navbar">
      <h1 class="logo">Mi Proyecto</h1>
      <ul class="nav-links" id="navLinks">
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#descripcion">Descripción</a></li>
        <li><a href="#tecnologias">Tecnologías</a></li>
        <li><a href="#galeria">Galería</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
      <div class="menu-toggle" id="menuToggle">&#9776;</div>
    </nav>
  </header>

  <!-- HERO -->
  <section id="inicio" class="hero">
    <div class="hero-content">
      <h2>Proyecto de Innovación Tecnológica</h2>
      <p>Una solución eficiente para la gestión de procesos en organizaciones modernas, integrando metodologías ágiles y herramientas tecnológicas avanzadas.</p>
      <a href="#descripcion" class="btn">Ver más</a>
    </div>
  </section>

  <!-- DESCRIPCIÓN -->
  <section id="descripcion" class="section">
    <h3>Descripción del Proyecto</h3>
    <p>
      Este proyecto busca optimizar la gestión de recursos y la comunicación dentro de equipos multidisciplinarios mediante una plataforma web intuitiva y escalable.
      Incluye módulos de colaboración, seguimiento de tareas y análisis de rendimiento en tiempo real.
    </p>
  </section>

  <!-- TECNOLOGÍAS -->
  <section id="tecnologias" class="section bg-light">
    <h3>Tecnologías Utilizadas</h3>
    <div class="tech-container">
      <div class="tech-card">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968267.png" alt="HTML">
        <p>HTML5</p>
      </div>
      <div class="tech-card">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968242.png" alt="CSS">
        <p>CSS3</p>
      </div>
      <div class="tech-card">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968292.png" alt="JavaScript">
        <p>JavaScript</p>
      </div>
      <div class="tech-card">
        <img src="https://cdn-icons-png.flaticon.com/512/5968/5968672.png" alt="Python">
        <p>Python</p>
      </div>
    </div>
  </section>

  <!-- GALERÍA -->
  <section id="galeria" class="section">
    <h3>Galería del Proyecto</h3>
    <div class="gallery">
      <img src="https://picsum.photos/400/250?random=1" alt="Imagen 1">
      <img src="https://picsum.photos/400/250?random=2" alt="Imagen 2">
      <img src="https://picsum.photos/400/250?random=3" alt="Imagen 3">
    </div>
  </section>

  <!-- CONTACTO -->
  <section id="contacto" class="section bg-light">
    <h3>Contacto</h3>
    <p>¿Deseas saber más sobre este proyecto o colaborar en una iniciativa similar?</p>
    <form class="contact-form">
      <input type="text" placeholder="Tu nombre" required>
      <input type="email" placeholder="Tu correo" required>
      <textarea placeholder="Tu mensaje" required></textarea>
      <button type="submit" class="btn">Enviar</button>
    </form>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>&copy; 2025 Jairo Armando Salcedo Aranda | Portafolio del Proyecto</p>
  </footer>

  <script>
    // --- MENÚ RESPONSIVO ---
    const menuToggle = document.getElementById('menuToggle');
    const navLinks = document.getElementById('navLinks');

    menuToggle.addEventListener('click', () => {
      navLinks.classList.toggle('show');
    });

    // --- FORMULARIO SIMULADO ---
    const form = document.querySelector('.contact-form');
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      alert('¡Gracias por tu mensaje! Te contactaremos pronto.');
      form.reset();
    });
  </script>

</body>
</html>
