<script>
  import { produtosAcademia } from '$lib/produtos.js';

  let produtosFiltrados = produtosAcademia.slice();
</script>

<!-- Contêiner principal com fundo cinza escuro -->
<div class="main-container">
  <!-- Exibição dos produtos -->
  <div class="row g-4">
    {#each produtosFiltrados as produto}
      <div class="col-md-6 col-xl-3">
        <div class="card h-100">
          <div class="row g-0">
            <div class="col-12">
              <img src={produto.imagem} class="img-fluid rounded-start produto-imagem" alt="imagem do produto" />
            </div>
            <div class="col-sm-8">
              <div class="card-body">
                <h5 class="card-title">{produto.nome}</h5>
                <h6 class="card-subtitle mb-2 text-body-secondary">Preço: {produto.preço}</h6>
                {#if produto.validade}
                  <p class="card-text">Validade: {produto.validade}</p>
                {/if}
                <p class="card-text categorias">
                  {#each produto.categorias as categoria}
                    <span class="badge text-bg-secondary mx-1">{categoria}</span>
                  {/each}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    {/each}
  </div>
</div>

<style>
  /* Aplicando o fundo cinza escuro no contêiner principal */
  .main-container {
    background-color: #333;  /* Cor de fundo cinza escuro */
    margin: 0;
    padding: 20px;
    height: 100vh;  /* Garante que o fundo cubra toda a altura da página */
  }

  /* Adicionando a cor de fundo cinza claro atrás das imagens e texto */
  .card-body {
    background-color: #f4f4f4;  /* Cor de fundo cinza claro */
    padding: 20px;
    border-radius: 10px;
  }

  .produto-imagem {
    max-width: 100%;        /* A imagem ocupa 100% da largura disponível */
    height: auto;           /* Mantém a proporção da imagem */
    object-fit: cover;      /* Faz com que a imagem cubra o espaço disponível sem distorcer */
    max-height: 250px;      /* Define a altura máxima das imagens */
    margin-bottom: 15px;    /* Espaço entre as imagens */
  }

  /* Layout para as imagens e cartões */
  .row.g-4 {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;  /* Adiciona espaçamento entre as colunas */
    margin: 0;  /* Remove margens extras */
  }

  /* Definir número de colunas por linha */
  .col-md-6 {
    flex: 1 1 calc(25% - 20px); /* Define as colunas em 4 por linha (25% da largura) */
  }

  @media (max-width: 768px) {
    .col-md-6 {
      flex: 1 1 calc(50% - 20px); /* Duas colunas em telas menores */
    }
  }

  @media (max-width: 576px) {
    .col-md-6 {
      flex: 1 1 calc(100% - 20px); /* Uma coluna por vez em telas ainda menores */
    }
  }

  /* Estilizando o título e o texto abaixo das imagens */
  .card-title {
    font-family: 'Poppins', sans-serif; /* Fonte mais moderna e legível */
    font-size: 1.25rem;  /* Tamanho de fonte ajustado */
    font-weight: 600;    /* Deixa o título mais forte */
  }

  .card-subtitle {
    font-family: 'Roboto', sans-serif; /* Fonte clean e legível */
    font-size: 1rem;   /* Tamanho de fonte ajustado */
    color: #666;       /* Cor de texto secundário */
  }

  .card-text {
    font-size: 14px;
    font-family: 'Roboto', sans-serif; /* Fonte moderna e clean */
    color: #333;
  }

  .categorias {
    font-size: 14px;
    margin-top: 10px;
  }

  /* Ajustando a aparência dos badges de categorias */
  .badge {
    font-size: 13px;
    font-family: 'Roboto', sans-serif;
    background-color: #e0e0e0; /* Cor de fundo dos badges */
    color: #333;  /* Cor do texto dos badges */
  }
</style>
