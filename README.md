<!DOCTYPE html>
<html lang="es">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Reserva hoteles, tours, seguros de viaje, alojamientos, alquiler de vehículos y traslados con facilidad y seguridad.">
  <title>Ecommerce Bueno Hotel</title>
  <link rel="icon" type="image/png" href="https://static-ecommerce.buenohotel.com.do/favicon.ico">
  <style>
    /* General Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* Body */
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      line-height: 1.6;
    }

    /* Header */
    header {
      background-color: #2c3e50;
      color: white;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    .logo-container img {
      height: 50px;
    }

    nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    nav ul li {
      margin: 0;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      cursor: pointer;
      font-size: 1rem;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(120deg, #fbb03b, #ff7700);
      color: white;
      text-align: center;
      padding: 30px 20px;
    }

    .hero h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 1.2em;
      margin-bottom: 20px;
    }

    .hero .btn {
      background-color: #1d23c5;
      color: white;
      padding: 15px 30px;
      border-radius: 5px;
      text-decoration: none;
      font-size: 1em;
      transition: background-color 0.3s ease;
      cursor: pointer;
    }

    .hero .btn:hover {
      background-color: #444;
    }

    /* Content Section */
    .content {
      text-align: center;
      padding: 40px 20px;
    }

    .content h2 {
      font-size: 2em;
      margin-bottom: 20px;
      color: #333;
    }

    /* Servicios */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      justify-content: center;
      align-items: stretch;
    }

    .service {
      background: white;
      border: 2px solid #007bff;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      padding: 20px;
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .service h3 {
      font-size: 1.4em;
      margin-bottom: 10px;
      color: #007bff;
    }

    .service p {
      color: #555;
      font-size: 1em;
    }

    /* Footer */
    footer {
      background-color: #2c3e50;
      color: white;
      text-align: center;
      padding: 20px;
    }

    footer p {
      margin: 0;
    }

    /* Media Queries */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }

      nav ul {
        justify-content: center;
        flex-wrap: wrap;
        gap: 5px;
      }

      .hero h1 {
        font-size: 2em;
      }

      .hero p {
        font-size: 1em;
      }

      .hero .btn {
        padding: 10px 20px;
      }
    }

    @media (max-width: 480px) {
      .hero h1 {
        font-size: 1.8em;
      }

      .hero p {
        font-size: 0.9em;
      }

      nav ul li a {
        font-size: 0.9rem;
      }

      .service h3 {
        font-size: 1.2em;
      }
    }
  </style>
</head>

<body>
  <header>
    <div class="logo-container">
      <img src="https://static-www.buenohotel.com.do/images/logo.png" alt="Logo de Bueno Hotel">
    </div>
    <nav>
      <ul>
        <li><a id="inicio-btn">Inicio</a></li>
        <li><a id="servicios-btn">Servicios</a></li>
        <li><a id="contacto-btn">Contactos</a></li>
        <li><a id="tienda-btn">Tienda</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h1>Bienvenidos a nuestra tienda de viajes</h1>
    <p>Reserva tus vacaciones soñadas con solo unos clicks.</p>
    <a id="explorar-btn" class="btn">Explorar</a>
  </section>

  <section id="servicios-section" class="content">
    <h2>Servicios Destacados</h2>
    <div class="services">
      <div class="service">
        <h3>🏨 Hoteles</h3>
        <p>Encuentra los mejores hoteles para tu descanso.</p>
      </div>
      <div class="service">
        <h3>🌍 Tours</h3>
        <p>Explora nuevos destinos con nuestros tours guiados.</p>
      </div>
      <div class="service">
        <h3>🛡️ Seguros de Viaje</h3>
        <p>Viaja con tranquilidad con nuestros seguros.</p>
      </div>
      <div class="service">
        <h3>🏠 Alojamientos</h3>
        <p>Opciones de alojamiento para todo tipo de viajes.</p>
      </div>
      <div class="service">
        <h3>🚗 Alquiler de Vehículos</h3>
        <p>Alquila el vehículo perfecto para tu viaje.</p>
      </div>
      <div class="service">
        <h3>🚕 Traslados</h3>
        <p>Reserva traslados confiables y cómodos.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2024 Bueno Hotel - Todos los derechos reservados</p>
  </footer>

  <script>
    // Funciones para los botones
    document.getElementById('inicio-btn').onclick = () => {
      alert("Volviendo al inicio...");
      window.scrollTo({ top: 0, behavior: 'smooth' });
    };

    document.getElementById('servicios-btn').onclick = () => {
      document.getElementById('servicios-section').scrollIntoView({ behavior: 'smooth' });
    };

    document.getElementById('contacto-btn').onclick = () => {
      alert("¡Ponte en contacto con nosotros! (Funcionalidad en desarrollo)");
    };

    document.getElementById('tienda-btn').onclick = () => {
      alert("Redirigiendo a la tienda... (Funcionalidad en desarrollo)");
    };

    document.getElementById('explorar-btn').onclick = () => {
      alert("Explorando servicios destacados...");
      document.getElementById('servicios-section').scrollIntoView({ behavior: 'smooth' });
    };
  </script>
</body>

</html>
