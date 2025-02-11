<script>
  const frases = [
    "💪 O suor de hoje é o sucesso de amanhã!",
    "🏋️‍♀️ Não desista, o progresso é um processo!",
    "🔥 A dor é temporária, o orgulho é para sempre!",
    "💥 Acredite em si mesmo, você pode mais do que imagina!",
    "🏋️‍♂️ Seu único limite é você!",
    "💪 Não pare até se orgulhar!",
    "🚀 Vencer é um hábito. Comece agora!",
    "🔥 O impossível só existe na sua mente!",
    "💥 O corpo alcança o que a mente acredita!",
    "🏋️‍♀️ Se você quer resultados, faça sacrifícios!",
    "💪 Hoje você vai além, não pare agora!",
    "🏅 Seus limites estão apenas no começo!",
    "💥 Desafie-se a ser melhor a cada dia!",
    "🔥 O sucesso não vem, você vai até ele!",
    "💪 A vitória é de quem nunca desiste!"
  ];
</script>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    height: 100vh;
    font-family: 'Impact', sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(45deg, rgb(255, 100, 100), rgb(100, 100, 255));
  }

  .container {
    width: 80%;
    max-width: 700px;
    text-align: center;
    padding-top: 50px;
  }

  .frase {
    margin-bottom: 20px;
    font-size: 1.5em;
    padding: 20px;
    border-radius: 10px;
    background: rgba(0, 0, 0, 0.6);
    color: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: all 0.3s ease-in-out;
  }

  .frase:hover {
    transform: scale(1.05);
    background: rgba(255, 255, 255, 0.2);
  }
</style>

<main>
  <div class="container">
    {#each frases as frase}
      <div class="frase">{frase}</div>
    {/each}
  </div>
</main>
