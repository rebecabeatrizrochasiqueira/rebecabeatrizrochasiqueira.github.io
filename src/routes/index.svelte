<script>
    let cores = [
      { nome: 'Vermelho', descricao: 'A cor mais intensa do arco-íris.' },
      { nome: 'Laranja', descricao: 'Uma mistura de vermelho e amarelo.' },
      { nome: 'Amarelo', descricao: 'Associada à luz e energia.' },
      { nome: 'Verde', descricao: 'Simboliza a natureza e a calma.' },
      { nome: 'Azul', descricao: 'Cor do céu e do mar.' },
      { nome: 'Anil', descricao: 'Tom profundo de azul.' },
      { nome: 'Violeta', descricao: 'Cor que representa espiritualidade.' },
    ];
  </script>
  
  <main>
    <h1>As Cores do Arco-íris</h1>
    <p>O arco-íris é composto por sete cores, que possuem significados e representações únicas.</p>
  
    <ul>
      {#each cores as cor}
        <li>
          <strong>{cor.nome}</strong>: {cor.descricao}
        </li>
      {/each}
    </ul>
  
    <nav>
      <a href="/sobre">Sobre</a> | <a href="/contato">Contato</a>
    </nav>
  </main>
  
  <style>
    main {
      text-align: center;
      padding: 20px;
    }
  
    h1 {
      color: #ff6347; /* cor de destaque */
    }
  
    a {
      text-decoration: none;
      color: #0000ff;
      margin: 0 10px;
    }
  
    a:hover {
      color: #ff6347;
    }
  
    ul {
      list-style-type: none;
    }
  
    li {
      margin: 10px 0;
    }
  </style>
  