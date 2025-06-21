# Psicoterritorio-web
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Psicoterritorio</title>
  <style>
    :root {
      --principal: #1e3a5f;
      --secundario: #f1f5f9;
      --detalle: #3b82f6;
      --fondo: #ffffff;
      --texto: #1f2937;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: var(--secundario);
      color: var(--texto);
    }

    header {
      background: linear-gradient(to right, var(--principal), #29507a);
      color: white;
      padding: 30px 20px;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: var(--principal);
      padding: 10px 0;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 20px;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: var(--detalle);
    }

    main {
      max-width: 1200px;
      margin: 40px auto;
      padding: 0 20px;
    }

    section {
      margin-bottom: 50px;
      background-color: var(--fondo);
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
    }

    section:hover {
      transform: scale(1.01);
    }

    h2 {
      color: var(--principal);
    }

    footer {
      background-color: var(--principal);
      color: white;
      text-align: center;
      padding: 20px;
    }

    form input, form select, form textarea {
      width: 100%;
      padding: 12px;
      margin: 8px 0 16px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 16px;
    }

    button {
      background-color: var(--detalle);
      color: white;
      padding: 12px 24px;
      font-size: 16px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #2563eb;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
    }

    th, td {
      border: 1px solid #ccc;
      padding: 12px;
      text-align: left;
    }

    th {
      background-color: #e2e8f0;
    }

    .imagen-destacada img {
      width: 100%;
      border-radius: 12px;
      margin-bottom: 20px;
    }

    .interactivo:hover {
      opacity: 0.9;
    }
  </style>
</head>
<body>
  <header>
    <h1>Psicoterritorio</h1>
    <p>Capacitaciones virtuales para profesionales de la salud en zonas rurales</p>
  </header>

  <nav>
    <a href="#sobre">Sobre</a>
    <a href="#temas">Temáticas</a>
    <a href="#capacitaciones">Capacitaciones</a>
    <a href="#eventos">Eventos</a>
    <a href="#inscripcion">Inscripción</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <main>
    <section id="sobre">
      <div class="imagen-destacada">
        <img src="https://via.placeholder.com/1200x400?text=Bienvenidos+a+Psicoterritorio" alt="Banner">
      </div>
      <h2>¿Qué es Psicoterritorio?</h2>
      <p>Psicoterritorio es una plataforma formativa creada a partir de experiencias reales de psicoeducación en comunidades rurales. Ahora convertida en un programa estructurado, ofrece capacitaciones virtuales especializadas para profesionales de la salud que trabajan en contextos rurales como Vilcabamba y Espíndola.</p>
    </section>

    <section id="temas">
      <h2>Temáticas Principales</h2>
      <ul>
        <li>Prevención de la violencia intrafamiliar y de género</li>
        <li>Intervención ante el abuso de sustancias psicoactivas</li>
        <li>Construcción de proyecto de vida en adolescentes</li>
        <li>Prevención del embarazo adolescente</li>
        <li>Salud mental comunitaria</li>
      </ul>
    </section>

    <section id="capacitaciones">
      <h2>Capacitaciones Virtuales</h2>
      <p>Las capacitaciones se realizan de forma 100% online con materiales descargables, tutorías en vivo, foros colaborativos y certificados digitales de participación.</p>
    </section>

    <section id="eventos">
      <h2>Calendario de Eventos</h2>
      <table>
        <tr>
          <th>Fecha</th>
          <th>Evento</th>
          <th>Modalidad</th>
        </tr>
        <tr>
          <td>10 julio 2025</td>
          <td>Taller de violencia y salud mental</td>
          <td>Online</td>
        </tr>
        <tr>
          <td>17 julio 2025</td>
          <td>Salud mental comunitaria: estrategias prácticas</td>
          <td>Online</td>
        </tr>
        <tr>
          <td>24 julio 2025</td>
          <td>Prevención del consumo en jóvenes rurales</td>
          <td>Online</td>
        </tr>
        <tr>
          <td>31 julio 2025</td>
          <td>Proyecto de vida en adolescencia</td>
          <td>Online</td>
        </tr>
        <tr>
          <td>07 agosto 2025</td>
          <td>Red de atención psicológica rural</td>
          <td>Online</td>
        </tr>
      </table>
    </section>

    <section id="inscripcion">
      <h2>Formulario de Inscripción</h2>
      <form>
        <label for="nombre">Nombre completo:</label>
        <input type="text" id="nombre" name="nombre" required>

        <label for="correo">Correo electrónico:</label>
        <input type="email" id="correo" name="correo" required>

        <label for="zona">Zona de trabajo:</label>
        <input type="text" id="zona" name="zona" placeholder="Ej. Vilcabamba, Espíndola">

        <label for="interes">Área de interés:</label>
        <select id="interes" name="interes">
          <option value="violencia">Violencia y género</option>
          <option value="sustancias">Abuso de sustancias</option>
          <option value="proyecto">Proyecto de vida</option>
          <option value="embarazo">Embarazo adolescente</option>
          <option value="salud">Salud mental</option>
        </select>

        <label for="mensaje">Comentarios adicionales:</label>
        <textarea id="mensaje" name="mensaje" rows="4"></textarea>

        <button type="submit">Enviar inscripción</button>
      </form>
    </section>

    <section id="contacto">
      <h2>Contacto</h2>
      <p>Escríbenos a: <strong>psicoterritorio@formacion.org</strong> para más información.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Psicoterritorio. Todos los derechos reservados.</p>
  </footer>
</body>
</html>
