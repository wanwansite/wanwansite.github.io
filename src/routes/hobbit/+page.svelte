<script>
  
</script>

<style>
  
  :global(body) {
    margin: 0;
    font-family: 'Arial', sans-serif;
    height: 100%;
    background-color: rgb(34, 139, 34);
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


  .button-container {
    position: fixed;
    top: 10px;
    left: 10px;
    right: 10px;
    display: flex;
    justify-content: space-between;
    width: calc(100% - 20px);
    z-index: 2;
  }

  .button-container a {
    background-color: #f1c40f;
    color: white;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
  }

  .button-container a:hover {
    background-color: #e67e22;
  }
</style>


<div class="button-container">

  <a href="https://wanwansite.github.io/">Home</a>


  <a href="https://wanwansite.github.io/senhor">Anéis</a>
</div>

<div class="container">
  <h1 class="titulo">O Hobbit</h1>

  <div class="personagens">
  
    <div class="card">
      <img src="https://ufmg.br/thumbor/0k4CbZ2F7V807pwjDMX2cxCnkWc=/0x0:1505x1003/712x474/https://ufmg.br/storage/a/7/c/b/a7cb5c6e5760c5ce1590752e9ac5ae41_15077319251864_980465810.jpg" alt="Bilbo Baggins" />
      <h3>Bilbo Baggins/Bolseiro</h3>
      <p>Bilbo é um hobbit que se vê envolvido em uma grande aventura com anões e Gandalf para recuperar um tesouro guardado por um dragão. Apesar de ser inicialmente relutante, Bilbo prova ser um herói em sua jornada e o anél do poder.</p>
    </div>

   
    <div class="card">
      <img src="https://multiversonoticias.com.br/wp-content/uploads/2023/11/galadriel-senhor-dos-aneis-olhar.png" alt="Gandalf" />
      <h3>Senhora Galadriel</h3>
      <p>Galadriel, uma elfa super poderosa que está presente nas duas triologias, ela é maravilhosamente linda encanta a todos, mas também ela dá um medinho.</p>
    </div>


    <div class="card">
      <img src="https://leitorcabuloso.com.br/wp-content/uploads/2014/04/thcc_thorin_01.jpg" alt="Thorin" />
      <h3>Thorin Escudo de Carvalho</h3>
      <p>Thorin é o líder dos anões que embarcam na jornada para recuperar a Montanha Solitária e o tesouro roubado pelo dragão Smaug. Seu senso de honra e coragem o tornam um líder imponente, embora sua ganância também seja um grande obstáculo.</p>
    </div>

 
    <div class="card">
      <img src="https://br.web.img3.acsta.net/c_300_300/img/68/61/68617d596b1868ea8b4b165848059e49.jpg" alt="Legolas" />
      <h3>Gollum</h3>
      <p>Gollum foi um ex-Hobbit, que após encontar o anel em um lago em seu aniversário e matar seu melhor amigo por ele, ficou maluco, e embora ele tenha criado uma bipolaridade, Gollum foi importante em toda triologia Hobbit e Senhor dos Anéis.</p>
    </div>

   
    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT_dHN1W8e9EXVYMBRMgfzg_hZr1N30yyRfhw&s" alt="Fili" />
      <h3>Fili</h3>
      <p>Fili é um dos anões da companhia de Thorin e um guerreiro corajoso. Ele é irmão de Kili e tem um forte senso de lealdade e é muito mais pé no chão do que o irmão, talvez porque ele fosse o primeiro na linha de sucessão depois de Thorin, sendo um dos principais lutadores na missão para derrotar Smaug.(e com certeza ele é o meu favorito entre os irmãos)</p>
    </div>

    
    <div class="card">
      <img src="https://i.pinimg.com/474x/13/e5/1b/13e51b7b75539506024e48c8668ad576.jpg" alt="Kili" />
      <h3>Kili</h3>
      <p>Kili é o irmão de Fili e um dos anões aventureiros que se juntam à missão para recuperar a Montanha Solitária. Ele é jovem, mas destemido e habilidoso com o arco e flecha, também se apaixonou por uma elfa, que no começo não dava muita bola para ele, porém depois no último filme ele acaba morrendo para proteger sua amada.</p>
    </div>

   
    <div class="card">
      <img src="https://preview.redd.it/1qlkz6mqcwpa1.jpg?auto=webp&s=2f1140b9fba196e472805d90cfb10d67918c0ae8" alt="Bard" />
      <h3>Bard, o Arqueiro</h3>
      <p>Bard é um arqueiro habilidoso de Lake-town (Esgaroth). Ele se torna um herói ao matar Smaug com uma flecha certeira, salvando a cidade e ajudando os povos da Terra-média a resistir à ameaça do dragão.</p>
    </div>
  </div>

  <div class="descricao">
    <h2>A Jornada de Bilbo Baggins</h2>
    <p>A história de O Hobbit segue a jornada de Bilbo Baggins/Bolseiro, um hobbit comum que é escolhido para se juntar a uma companhia de anões e ao mago Gandalf em uma missão para recuperar um tesouro guardado pelo dragão Smaug. Ao longo dessa jornada, Bilbo enfrenta desafios perigosos e aprende muito sobre coragem, lealdade e amizade. A busca por esse tesouro acaba se tornando muito mais do que o simples enriquecimento material – ela é uma luta pela liberdade e pela justiça contra forças que ameaçam a Terra-média.</p>
  </div>
</div>
