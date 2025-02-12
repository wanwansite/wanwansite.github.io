<script>
    // Lógica de script aqui, se necessário
  </script>
  
  <style>
    /* Garantir que o body e html cubram toda a altura da tela */
  
    .fundo {
      background-color: rgb(255, 236, 204);
      padding: 0;
      height: 100vh; /* Garantir que o fundo cubra 100% da altura da tela */
      display: flex;
      justify-content: center; /* Centraliza o conteúdo horizontalmente */
      align-items: center; /* Centraliza o conteúdo verticalmente */
      margin: 0;
      position: relative; /* Necessário para o posicionamento absoluto da imagem */
    }
  
    .conteudo {
      text-align: center; /* Centraliza o texto */
      padding: 20px; /* Espaçamento interno no retângulo */
      background-color: white; /* Fundo branco para dar destaque */
      border-radius: 10px; /* Bordas arredondadas no retângulo */
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1); /* Sombra sutil para destacar */
      z-index: 1; /* Garante que o conteúdo fique acima da imagem */
    }
  
    .logo {
      position: absolute; 
      top: 50%; /* Centraliza verticalmente */
      left: 50%; /* Centraliza horizontalmente */
      transform: translate(-50%, -50%); /* Ajuste fino para centralizar */
      z-index: 0; /* A logo vai ficar atrás do conteúdo */
    }
  
    .logo img {
      max-width: 100%;
      height: auto;
      width: 800px; /* Ajuste o tamanho da imagem conforme necessário */
    }
  
    .texto-bem-vindo {
      color: rgb(19, 18, 18); /* Cor do texto */
      font-size: 2rem; /* Tamanho do texto */
      margin-bottom: 20px; /* Espaçamento abaixo do texto */
    }
  
    .botao {
      margin-top: 20px; /* Espaçamento superior para o botão */
    }
  </style>
  
  <div class="fundo">
    <div class="conteudo">
      <!-- Texto acima do botão -->
      <p class="texto-bem-vindo">Conheça meus personagens favoritos do filme Senhor dos Anéis</p>
  
      <!-- Botão Bootstrap -->
      <a href="http://localhost:5174/pag2" class="btn btn-primary botao">PERSONAGENS</a>
    </div>
  </div>
  
  <div class="logo">
    <img src="/Design sem nome.png" class="img-fluid" alt="Logo">
  </div>