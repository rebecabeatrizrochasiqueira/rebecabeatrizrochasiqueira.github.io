<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sobre o Arco-íris</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: #333;
      background-image: url('https://img.freepik.com/fotos-gratis/beleza-da-natureza-no-ceu-do-sol-da-estratosfera-da-luz-solar-azul-gerado-pela-ia_188544-19779.jpg');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      text-align: center;
    }

    main {
      background: rgba(255, 255, 255, 0.8);
      margin: 50px auto;
      padding: 20px;
      border-radius: 10px;
      max-width: 800px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    h1 {
      color: #000000 ;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.2em;
      line-height: 1.6;
    }

    nav {
      margin-top: 20px;
    }

    a {
      text-decoration: none;
      color: #0000ff;
      font-weight: bold;
      margin: 0 10px;
    }

    a:hover {
      color: #32cd32;
    }

    footer {
      margin-top: 40px;
      padding: 10px 0;
      background: rgba(0, 0, 0, 0.5);
      color: #fff;
      font-size: 0.9em;
    }
  </style>
</head>
<body>
  <script>
    let descricao = "O arco-íris é um fenômeno óptico e meteorológico que resulta da reflexão, refração e dispersão da luz em gotículas de água, criando um espectro de luz visível no céu.";
     document.getElementById("descricao").innerText = descricao;
 </script>

  <main>
    <h1>Sobre o Arco-íris</h1>
    <p id="descricao"></p>

    <nav>
      <a href="/">Página Inicial</a> | <a href="/contato">Contato</a>
    </nav>
  </main>

  <footer>
    © 2025 - Sua Página sobre Arco iris 
  </footer>

</body>
</html>