<script>
  // Lógica de script aqui, se necessário
</script>

<style>
  /* Adicionando um fundo verde RGB ao body, garantindo que fique atrás de tudo */
  :global(body) {
    margin: 0;
    font-family: 'Arial', sans-serif;
    height: 100%;
    background-color: rgb(34, 139, 34); /* Cor verde RGB */
    position: relative;
    z-index: -1; /* Garante que o fundo fique atrás de tudo */
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
    z-index: 1; /* Garantir que o conteúdo da página apareça acima do fundo */
    position: relative;
  }

  /* Título */
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
    background-color: #34495e; /* Fundo de cada card */
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s;
  }

  .card:hover {
    transform: scale(1.05); /* Efeito de hover para aumentar o card */
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

  /* Estilos para as descrições */
  .descricao {
    margin-top: 30px;
    font-size: 1.2rem;
    color: #ecf0f1;
    text-align: justify;
  }
</style>

<div class="container">
  <h1 class="titulo">Os Heróis de O Hobbit</h1>

  <div class="personagens">
    <!-- Card do Bilbo -->
    <div class="card">
      <img src="https://ufmg.br/thumbor/0k4CbZ2F7V807pwjDMX2cxCnkWc=/0x0:1505x1003/712x474/https://ufmg.br/storage/a/7/c/b/a7cb5c6e5760c5ce1590752e9ac5ae41_15077319251864_980465810.jpg" alt="Bilbo Baggins" />
      <h3>Bilbo Baggins</h3>
      <p>Bilbo é um hobbit que se vê envolvido em uma grande aventura com anões e Gandalf para recuperar um tesouro guardado por um dragão. Apesar de ser inicialmente relutante, Bilbo prova ser um herói em sua jornada.</p>
    </div>

    <!-- Card do Gandalf -->
    <div class="card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/e/ef/Gandalf_%28Ian_McKellen%29_%28The_Hobbit%29.jpg" alt="Gandalf" />
      <h3>Gandalf, o Cinzento</h3>
      <p>Gandalf é um mago que ajuda Bilbo e os anões em sua jornada para recuperar o tesouro do dragão Smaug. Ele é sábio e poderoso, com grande influência nas decisões que moldam o destino da Terra-média.</p>
    </div>

    <!-- Card do Thorin -->
    <div class="card">
      <img src="https://leitorcabuloso.com.br/wp-content/uploads/2014/04/thcc_thorin_01.jpg" alt="Thorin" />
      <h3>Thorin Escudo de Carvalho</h3>
      <p>Thorin é o líder dos anões que embarcam na jornada para recuperar a Montanha Solitária e o tesouro roubado pelo dragão Smaug. Seu senso de honra e coragem o tornam um líder imponente, embora sua ganância também seja um grande obstáculo.</p>
    </div>

    <!-- Card do Legolas -->
    <div class="card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/d/df/Legolas_%28Orlando_Bloom%29_%28The_Hobbit%29.jpg" alt="Legolas" />
      <h3>Legolas</h3>
      <p>Legolas é um elfo da Floresta das Trevas e amigo leal de Thorin. Ele é um arqueiro excepcional e combate com grande destreza, sempre pronto para lutar ao lado de seus amigos na jornada.</p>
    </div>

    <!-- Card do Fili -->
    <div class="card">
      <img src="00https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT_dHN1W8e9EXVYMBRMgfzg_hZr1N30yyRfhw&s" alt="Fili" />
      <h3>Fili</h3>
      <p>Fili é um dos anões da companhia de Thorin e um guerreiro corajoso. Ele é irmão de Kili e tem um forte senso de lealdade, sendo um dos principais lutadores na missão para derrotar Smaug.</p>
    </div>

    <!-- Card do Kili -->
    <div class="card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Kili_%28The_Hobbit%29.jpg" alt="Kili" />
      <h3>Kili</h3>
      <p>Kili é o irmão de Fili e um dos anões aventureiros que se juntam à missão para recuperar a Montanha Solitária. Ele é jovem, mas destemido e habilidoso com o arco e flecha, além de ser leal à sua companhia.</p>
    </div>

    <!-- Card do Bard -->
    <div class="card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/9/92/Bard_the_Bowman_%28Luke_Evans%29.jpg" alt="Bard" />
      <h3>Bard, o Arqueiro</h3>
      <p>Bard é um arqueiro habilidoso de Lake-town (Esgaroth). Ele se torna um herói ao matar Smaug com uma flecha certeira, salvando a cidade e ajudando os povos da Terra-média a resistir à ameaça do dragão.</p>
    </div>

  </div>

  <div class="descricao">
    <h2>A Jornada de Bilbo Baggins</h2>
    <p>A história de O Hobbit segue a jornada de Bilbo Baggins, um hobbit comum que é escolhido para se juntar a uma companhia de anões e ao mago Gandalf em uma missão para recuperar um tesouro guardado pelo dragão Smaug. Ao longo dessa jornada, Bilbo enfrenta desafios perigosos e aprende muito sobre coragem, lealdade e amizade. A busca por esse tesouro acaba se tornando muito mais do que o simples enriquecimento material – ela é uma luta pela liberdade e pela justiça contra forças que ameaçam a Terra-média.</p>
  </div>
  </div>