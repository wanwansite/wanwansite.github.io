<script>
  // Lógica de script aqui, se necessário
</script>

<style>
  .fundo {
    background-image: url('/floresta.jpg');
    background-size: cover;
    background-position: center;
    padding: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    position: relative;
  }

  .conteudo {
    text-align: center;
    padding: 30px;
    background-color: rgba(255, 255, 255, 0.7);
    border-radius: 10px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    z-index: 1;
  }

  .texto-bem-vindo {
    color: rgb(19, 18, 18);
    font-size: 2rem;
    font-family: 'Roboto', sans-serif;
    font-weight: bold;
    margin-bottom: 20px;
  }

  .botao {
    display: inline-block;
    margin-top: 20px;
    padding: 15px 30px;
    background-color: #4CAF50; /* Cor personalizada para o botão */
    color: white;
    font-size: 1.2rem; /* Tamanho de fonte maior */
    font-weight: bold;
    text-transform: uppercase; /* Maiúsculas no texto */
    border: none;
    border-radius: 30px; /* Bordas arredondadas */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Sombra para dar profundidade */
    text-decoration: none;
    transition: all 0.3s ease;
  }

  .botao:hover {
    background-color: #45a049; /* Cor do botão ao passar o mouse */
    transform: translateY(-5px); /* Leve efeito de "elevar" ao passar o mouse */
  }

  .botao:active {
    transform: translateY(2px); /* Efeito de pressionamento */
  }
</style>

<div class="fundo">
  <div class="conteudo">
    <p class="texto-bem-vindo">✨✨Conheça meus personagens favoritos dos meus filmes favoritos✨✨</p>
    <a href="https://wanwansite.github.io/senhor" class="botao">Senhor Dos Anéis</a>
    <a href="https://wanwansite.github.io/hobbit" class="botao">O Hobbit</a>
  </div>
</div>
