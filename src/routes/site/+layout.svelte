<script>
    import { onMount } from 'svelte';
    onMount(() => {
      document.title = 'Cores do Arco-íris';
    });
  </script>
  
  <header>
    <h1>O Arco-íris</h1>
    <nav>
      <a href="/">Página Inicial</a> | 
      <a href="/sobre">Sobre</a> | 
      <a href="/contato">Contato</a>
    </nav>
  </header>
  
  <main>
    <slot></slot> <!-- Este slot será substituído pelo conteúdo de cada página -->
  </main>
  
  <footer>
    <p>&copy; 2025 Arco-íris</p>
  </footer>
  
  <style>
    header, footer {
      text-align: center;
      padding: 10px;
      background-color: #f0f8ff;
    }
  
    nav a {
      margin: 0 15px;
      color: #4682b4;
      text-decoration: none;
    }
  
    nav a:hover {
      color: #ff6347;
    }
  
    footer {
      font-size: 12px;
      color: #888;
    }
  </style>
  