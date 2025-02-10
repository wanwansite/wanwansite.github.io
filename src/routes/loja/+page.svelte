<script>
  import { produtosAcademia } from '$lib/produtos.js';

  let produtosFiltrados = $state(produtosAcademia.slice());
  let categoriasSelecionadas = $state([]);

  // Função de filtro de categorias
  function filtrarCategorias(event) {
    if (event.target.checked) {
      categoriasSelecionadas.push(event.target.value);
    } else {
      categoriasSelecionadas.splice(categoriasSelecionadas.indexOf(event.target.value), 1);
    }

    if (categoriasSelecionadas.length == 0) {
      produtosFiltrados = produtosAcademia.slice();
    } else {
      produtosFiltrados = [];
      for (const produto of produtosAcademia) {
        for (const categoria of categoriasSelecionadas) {
          if (produto.categorias && produto.categorias.includes(categoria)) {
            produtosFiltrados.push(produto);
            break;
          }
        }
      }
    }
  }
</script>

<div class="row align-items-center mb-3">
  <div class="col-md-4"><input class="form-control" placeholder="Filtrar..." /></div>
  {#each ["Suplementos", "Acessórios", "Vestuário"] as categoria}
    <div class="col">
      <div class="form-check form-check-inline">
        <input type="checkbox" oninput={filtrarCategorias} class="form-check-input" id={categoria} value={categoria} />
        <label class="form-check-label" for={categoria}>{categoria}</label>
      </div>
    </div>
  {/each}
</div>

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

<style>
  /* Garantir que as imagens de produto fiquem do mesmo tamanho */
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

  /* Estilizando o texto abaixo das imagens */
  .card-text {
    font-size: 16px;
    font-family: 'Arial', sans-serif; /* Fonte mais moderna */
    margin-top: 10px;
  }

  .categorias {
    font-size: 14px;
  }

  /* Ajustando a aparência dos badges de categorias */
  .badge {
    font-size: 13px;
  }
</style>
