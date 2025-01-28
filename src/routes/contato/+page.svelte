<script>
  let nome = '';
  let email = '';
  let mensagem = '';

  function enviarMensagem() {
    if (nome && email && mensagem) {
      alert('Contato salvo! Que seu dia seja radiante igual o arco-íris!');
      nome = '';
      email = '';
      mensagem = '';
    } else {
      alert('Por favor, preencha todos os campos.');
    }
  }
</script>

<main>
  <h1 class="rainbow-text">
    <span>Contato</span>
  </h1>
  
  <form on:submit|preventDefault={enviarMensagem}>
    <label for="nome" class="rainbow-text">Nome:</label>
    <input id="nome" type="text" bind:value={nome} required class="input-rainbow" />

    <label for="email" class="rainbow-text">E-mail:</label>
    <input id="email" type="email" bind:value={email} required class="input-rainbow" />

    <label for="mensagem" class="rainbow-text">Mensagem:</label>
    <textarea id="mensagem" bind:value={mensagem} required class="input-rainbow"></textarea>

    <button type="submit" class="rainbow-button">Enviar</button>
  </form>

  <nav>
    <a href="/">Página Inicial</a> | <a href="/sobre">Sobre</a>
  </nav>
</main>

<style>
  body {
    background-color: #f0f8ff;
    font-family: Arial, sans-serif;
    border: 5px solid transparent;
    animation: border-color-change 10s infinite;
  }

  @keyframes border-color-change {
    0% { border-color: #FF0000; }
    14% { border-color: #FF7F00; }
    28% { border-color: #FFFF00; }
    42% { border-color: #00FF00; }
    57% { border-color: #0000FF; }
    71% { border-color: #4B0082; }
    85% { border-color: #8B00FF; }
    100% { border-color: #FF0000; }
  }

  main {
    text-align: center;
    padding: 20px;
  }

  h1 {
    font-size: 2em;
    text-shadow: 2px 2px #FFD700;
  }

  .rainbow-text {
    animation: color-change 10s infinite;
  }

  @keyframes color-change {
    0% { color: #FF0000; }
    14% { color: #FF7F00; }
    28% { color: #FFFF00; }
    42% { color: #00FF00; }
    57% { color: #0000FF; }
    71% { color: #4B0082; }
    85% { color: #8B00FF; }
    100% { color: #FF0000; }
  }

  form {
    margin: 20px auto;
    max-width: 300px;
    text-align: left;
    background-color: #ffffff;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }

  label {
    display: block;
    margin-top: 10px;
    color: transparent;
    font-weight: bold;
    animation: text-color-change 10s infinite;
    background-clip: text;
    -webkit-background-clip: text;
  }

  .input-rainbow {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 2px solid transparent;
    border-radius: 5px;
    background-color: #000;
    color: transparent;
    animation: text-color-change 10s infinite;
    background-clip: text;
    -webkit-background-clip: text;
  }

  @keyframes text-color-change {
    0% { color: #FF0000; }
    14% { color: #FF7F00; }
    28% { color: #FFFF00; }
    42% { color: #00FF00; }
    57% { color: #0000FF; }
    71% { color: #4B0082; }
    85% { color: #8B00FF; }
    100% { color: #FF0000; }
  }

  button {
    margin-top: 10px;
    padding: 10px;
    border: none;
    color: white;
    cursor: pointer;
    font-weight: bold;
    text-transform: uppercase;
    border-radius: 5px;
    box-shadow: 0 0 5px;
    animation: rainbow-glow 2s infinite;
    background: linear-gradient(45deg, #FF0000, #FF7F00, #FFFF00, #00FF00, #0000FF, #4B0082, #8B00FF);
    background-size: 400% 400%;
  }

  @keyframes rainbow-glow {
    0% { box-shadow: 0 0 10px #FF0000; }
    14% { box-shadow: 0 0 10px #FF7F00; }
    28% { box-shadow: 0 0 10px #FFFF00; }
    42% { box-shadow: 0 0 10px #00FF00; }
    57% { box-shadow: 0 0 10px #0000FF; }
    71% { box-shadow: 0 0 10px #4B0082; }
    85% { box-shadow: 0 0 10px #8B00FF; }
    100% { box-shadow: 0 0 10px #FF0000; }
  }

  a {
    text-decoration: none;
    color: #0000ff;
    margin: 0 10px;
  }

  a:hover {
    color: #4682b4;
  }
</style>



