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
    font-size: 2rem; /* Diminuí o tamanho da fonte */
    font-family: 'Roboto', sans-serif;
    font-weight: bold;
    margin-bottom: 20px;
  }

  .botao {
    margin-top: 20px;
  }
</style>

<div class="fundo">
  <div class="conteudo">
    <p class="texto-bem-vindo">Conheça meus personagens favoritos do filme Senhor dos Anéis</p>
    <a href="http://localhost:5173/senhor" class="btn btn-primary botao">PERSONAGENS</a>
  </div>
</div>
