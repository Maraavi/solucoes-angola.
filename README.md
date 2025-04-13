# solucoes-angola.
Site institucional da empresa Soluções Angola
<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Soluções Angola</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f8f9fa;
    }
    header {
      background: linear-gradient(to right, #00c9ff, #92fe9d);
      color: white;
      padding: 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    .logo {
      font-weight: bold;
      font-size: 1.4em;
    }
    .menu {
      display: flex;
      gap: 20px;
    }
    .menu button {
      background: white;
      border: none;
      padding: 10px 20px;
      border-radius: 5px;
      color: #007b8a;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s;
    }
    .menu button:hover {
      background: #e0f7fa;
    }
    section {
      display: none;
      padding: 20px;
      animation: fade 0.5s ease-in-out;
    }
    section.active {
      display: block;
    }
    @keyframes fade {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    footer {
      background: #007b8a;
      color: white;
      text-align: center;
      padding: 10px;
    }
    .contactos a {
      color: white;
      text-decoration: none;
      margin: 0 10px;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">Soluções Angola</div>
    <div class="menu">
      <button onclick="mostrarSecao('quem-somos')">Quem Somos?</button>
      <button onclick="mostrarSecao('servicos')">Serviços</button>
      <button onclick="mostrarSecao('portfolio')">Portfólio</button>
      <button onclick="mostrarSecao('testemunhos')">Testemunhos</button>
    </div>
  </header>

  <section id="quem-somos" class="active">
    <h2>Quem Somos?</h2>
    <p>Somos especialistas em limpeza profissional. Soluções à sua medida com excelência em cada detalhe.</p>
  </section>

  <section id="servicos">
    <h2>Serviços</h2>
    <ul>
      <li>Limpeza residencial</li>
      <li>Limpeza comercial</li>
      <li>Limpeza pós-obra</li>
      <li>Manutenção de espaços</li>
    </ul>
  </section>

  <section id="portfolio">
    <h2>Portfólio</h2>
    <p>Veja alguns dos nossos trabalhos realizados em empresas, residências e obras.</p>
  </section>

  <section id="testemunhos">
    <h2>Testemunhos</h2>
    <p>"Excelente serviço, muito profissionais!" - Cliente A</p>
    <p>"Confio sempre na Soluções Angola para limpar o meu escritório." - Cliente B</p>
  </section>

  <footer>
    <div class="contactos">
      <span>Contactos:</span>
      <a href="tel:+244900000000">+244 900 000 000</a> |
      <a href="mailto:info@solucoesangola.com">info@solucoesangola.com</a> |
      <a href="https://www.instagram.com/solucoesangola" target="_blank">Instagram</a>
    </div>
  </footer>

  <script>
    function mostrarSecao(id) {
      document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>