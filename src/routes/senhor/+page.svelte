<script>
  // Lógica de script aqui, se necessário
</script>

<style>
  :global(body) {
    margin: 0;
    font-family: 'Arial', sans-serif;
    height: 100%;
    background-color: rgb(34, 139, 34); /* Cor verde RGB */
    position: relative;
    z-index: -1;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
    z-index: 1;
    position: relative;
  }

  .titulo {
    text-align: center;
    font-size: 3rem;
    color: #f1c40f;
    margin-bottom: 40px;
    text-transform: uppercase;
    letter-spacing: 5px;
  }

  .personagens {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 30px;
    justify-items: center;
  }

  .card {
    background-color: #34495e;
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s;
  }

  .card:hover {
    transform: scale(1.05);
  }

  .card img {
    max-width: 100%;
    border-radius: 8px;
    height: 300px;
    object-fit: cover;
  }

  .card h3 {
    margin-top: 15px;
    font-size: 1.5rem;
    color: #f1c40f;
  }

  .card p {
    font-size: 1rem;
    color: #ecf0f1;
    margin-top: 10px;
  }

  .descricao {
    margin-top: 30px;
    font-size: 1.2rem;
    color: #ecf0f1;
    text-align: justify;
  }

  /* Botões Home e Hobbit no topo */
  .button-container {
    position: absolute;
    top: 10px;
    left: 10px;
    right: 10px;
    display: flex;
    justify-content: space-between;
    width: 100%;
    z-index: 2;
  }

  .botao-topo {
    background-color: #f39c12;
    color: white;
    padding: 10px 20px;
    font-size: 1rem;
    text-decoration: none;
    border-radius: 5px;
    text-transform: uppercase;
  }

  .botao-topo:hover {
    background-color: #e67e22;
  }

  /* Gandalf se movendo pela tela */
  .gandalf {
    position: absolute;
    top: 50%;
    left: -100px;
    animation: moverGandalf 10s linear infinite;
    z-index: 1;
  }

  @keyframes moverGandalf {
    0% {
      left: -100px;
    }
    50% {
      left: 50%;
      transform: translateX(-50%);
    }
    100% {
      left: 100%;
    }
  }
</style>

<div class="button-container">
  <a href="https://wanwansite.github.io/" class="botao-topo">Home</a>
  <a href="https://wanwansite.github.io/hobbit" class="botao-topo">Hobbit</a>
</div>

<div class="gandalf">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/53/Gandalf_the_Grey_-_The_Lord_of_the_Rings.jpg" alt="Gandalf" width="80" height="80" />
</div>

<div class="container">
  <h1 class="titulo">Senhor Dos Anéis</h1>

  <div class="personagens">
    <div class="card">
      <img src="https://pm1.aminoapps.com/6308/61e613bfde1b95f18e14afda9fa97215cd2ee6e4_00.jpg" alt="Frodo" />
      <h3>Frodo Bolseiro</h3>
      <p>Portador do Um Anel, Frodo é um hobbit corajoso, que embarca em uma jornada épica para destruir o Anel e salvar a Terra-média.</p>
    </div>

    <div class="card">
      <img src="https://www.factinate.com/storage/app/media/factinate/2018/01/Screenshot-2023-05-18-135739.jpg" alt="Aragorn" />
      <h3>Aragorn</h3>
      <p>O herdeiro de Isildur, Aragorn é um habilidoso ranger e o líder dos homens na batalha contra as forças de Sauron.</p>
    </div>

    <div class="card">
      <img src="https://rollingstone.com.br/media/uploads/gandolf_reproducao_widelg_1.jpg" alt="Gandalf" />
      <h3>Gandalf, o Cinzento</h3>
      <p>Um mago poderoso, Gandalf guia a Sociedade do Anel e é fundamental na luta contra as forças de Sauron, usando sua sabedoria e magia.</p>
    </div>

    <div class="card">
      <img src="https://newr7-r7-prod.web.arc-cdn.net/resizer/v2/6Z4SPZNDZBA5BF4VHE3GXSLSAU.jpg?auth=dfd60035062c9f48afd1780bc38fe828d15cb685e7e0ce0fe170ac584461ca33&width=1200&height=675" alt="Legolas" />
      <h3>Legolas</h3>
      <p>Elfo de Mirkwood, Legolas é um arqueiro excepcional e membro da Sociedade do Anel, lutando ao lado de seus amigos para proteger a Terra-média.</p>
    </div>

    <div class="card">
      <img src="https://p2.trrsf.com/image/fget/cf/774/0/images.terra.com/2023/10/02/128888124-05c0ab4f8e6801e0f74e0a37908bb3ae.jpg" alt="Gimli" />
      <h3>Gimli</h3>
      <p>O anão, filho de Glóin, é um guerreiro valente, membro da Sociedade do Anel, e tem uma amizade única com Legolas, o elfo.</p>
    </div>

    <div class="card">
      <img src="https://pm1.aminoapps.com/6303/7bc03d89e05c16e8865c3c6df1f385cc28555e9f_00.jpg" alt="Samwise" />
      <h3>Samwise Gamgee</h3>
      <p>Fiel amigo de Frodo, Sam é um hobbit determinado, que demonstra grande coragem e lealdade durante a jornada para destruir o Anel.</p>
    </div>

    <div class="card">
      <img src="https://i0.wp.com/graphicpolicy.com/wp-content/uploads/2021/10/OneDoesNotSimply.jpg?ssl=1" alt="Boromir" />
      <h3>Boromir</h3>
      <p>Filho de Denethor e herdeiro de Gondor, Boromir é um guerreiro valente, mas sua ambição com o Anel acaba colocando a Sociedade em risco.</p>
    </div>

    <div class="card">
      <img src="https://m.media-amazon.com/images/M/MV5BMzZmODdkMWQtNzUzMi00Yjg4LWJlYTYtZWQ2OGM2ODMzMTQyXkEyXkFqcGc@.V1.jpg" alt="Arwen" />
      <h3>Pippin Took</h3>
      <p>Pippin Took é um hobbit aventureiro e curioso, amigo de Frodo e membro da Sociedade do Anel.</p>
    </div>

    <div class="card">
      <img src="https://wallpapercat.com/w/full/1/1/e/3782583.jpg" alt="Gollum" />
      <h3>Merry - Meriadoc Brandebuque</h3>
      <p>Merry é um hobbit inteligente e leal, também membro da Sociedade do Anel.</p>
    </div>
  </div>

  <div class="descricao">
    <h2>A Jornada da Sociedade do Anel</h2>
    <p>A Sociedade do Anel foi formada com o objetivo de destruir o Um Anel...</p>
  </div>
</div>
