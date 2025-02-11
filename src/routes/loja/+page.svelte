<script>
  import { produtosAcademia } from '$lib/produtos.js';

  let produtosFiltrados = produtosAcademia.slice();

  function voltar() {
    window.location.href = "https://wanwansite.github.io/#";
  }

  function irParaFrases() {
    window.location.href = "https://wanwansite.github.io/frases";
  }
</script>

<div class="main-container">
  <div class="d-flex justify-content-between">
    <button class="btn btn-dark" on:click={voltar}>Voltar</button>
    <button class="btn btn-dark" on:click={irParaFrases}>Frases</button>
  </div>

  <div class="row g-4 mt-4">
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
                
                <a href={produto.referência} target="_blank" class="btn btn-link">Ver na loja</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    {/each}
  </div>
</div>

<style>
  .main-container {
    background-color: #ffffff;
    margin: 0;
    padding: 20px;
    height: 100vh;
  }

  .card-body {
    background-color: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
  }

  .produto-imagem {
    max-width: 100%;
    height: auto;
    object-fit: cover;
    max-height: 250px;
    margin-bottom: 15px;
  }

  .row.g-4 {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin: 0;
  }

  .col-md-6 {
    flex: 1 1 calc(25% - 20px);
  }

  @media (max-width: 768px) {
    .col-md-6 {
      flex: 1 1 calc(50% - 20px);
    }
  }

  @media (max-width: 576px) {
    .col-md-6 {
      flex: 1 1 calc(100% - 20px);
    }
  }

  .card-title {
    font-family: 'Poppins', sans-serif;
    font-size: 1.25rem;
    font-weight: 600;
  }

  .card-subtitle {
    font-family: 'Roboto', sans-serif;
    font-size: 1rem;
    color: #666;
  }

  .card-text {
    font-size: 14px;
    font-family: 'Roboto', sans-serif;
    color: #333;
  }

  .categorias {
    font-size: 14px;
    margin-top: 10px;
  }

  .badge {
    font-size: 13px;
    font-family: 'Roboto', sans-serif;
    background-color: #e0e0e0;
    color: #333;
  }

  .btn-link {
    padding: 0;
    text-decoration: none;
  }
</style>
