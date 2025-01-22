<script>
    let nome = '';
    let email = '';
    let mensagem = '';
  
    function enviarMensagem() {
      if (nome && email && mensagem) {
        alert('Mensagem enviada com sucesso!');
        nome = '';
        email = '';
        mensagem = '';
      } else {
        alert('Por favor, preencha todos os campos.');
      }
    }
  </script>
  
  <main>
    <h1>Contato</h1>
  
    <form on:submit|preventDefault={enviarMensagem}>
      <label for="nome">Nome:</label>
      <input id="nome" type="text" bind:value={nome} required />
  
      <label for="email">E-mail:</label>
      <input id="email" type="email" bind:value={email} required />
  
      <label for="mensagem">Mensagem:</label>
      <textarea id="mensagem" bind:value={mensagem} required></textarea>
  
      <button type="submit">Enviar</button>
    </form>
  
    <nav>
      <a href="/">Página Inicial</a> | <a href="/sobre">Sobre</a>
    </nav>
  </main>
  
  <style>
    main {
      text-align: center;
      padding: 20px;
    }
  
    h1 {
      color: #4682b4;
    }
  
    form {
      margin: 20px auto;
      max-width: 300px;
      text-align: left;
    }
  
    label {
      display: block;
      margin-top: 10px;
    }
  
    input, textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
    }
  
    button {
      margin-top: 10px;
      padding: 10px;
      background-color: #ff6347;
      border: none;
      color: white;
      cursor: pointer;
    }
  
    button:hover {
      background-color: #ff4500;
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
  