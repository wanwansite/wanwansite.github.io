<script>
    // Função para navegar para a loja (em uma aplicação real, você pode configurar o roteamento com o svelte-router)
    function irParaLoja() {
        window.location.href = "/loja"; // Aqui você redireciona para a página de loja
    }
</script>

<svelte:head>
    <style>
        /* Estilos globais - Garantir que o body e html ocupem toda a altura da tela */
        html, body {
            margin: 0;
            padding: 0;
            height: 100%; /* Garantir que a altura seja 100% */
        }

        /* Estilos globais para o fundo */
        .fundodosite {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif; /* Fonte moderna e grossa */
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start; /* Coloca o conteúdo mais próximo do topo */
            padding-top: 80px; /* Adiciona espaço no topo */
            background-color: #263238; /* Cor sólida de cinza escuro */
        }

        /* Estilo do título principal */
        h1 {
            font-size: 50px;
            font-weight: 700; /* Letras grossas */
            text-align: center;
            color: #fff; /* Cor do texto para contraste */
            margin-top: 0; /* Remove a margem superior do título */
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }

        /* Estilo para o quadrado branco de destaque */
        .text-box {
            background-color: rgb(255, 255, 255); /* Fundo branco */
            padding: 30px;
            border-radius: 15px; /* Bordas arredondadas */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 80%;
            max-width: 600px;
            text-align: center;
        }

        /* Estilo da segunda frase */
        .sub-title {
            font-size: 24px;
            font-weight: 600; /* Negrito */
            color: #333;
            margin-bottom: 20px;
        }

        /* Estilo do botão */
        button {
            background-color: rgb(221, 123, 67); /* Cor do botão */
            color: black;
            font-size: 18px;
            font-weight: 700;
            padding: 15px 30px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: rgb(255, 94, 0); /* Tom mais escuro ao passar o mouse */
        }
    </style>
</svelte:head>

<!-- Corpo da página home -->
<div class="fundodosite">
    <!-- Texto principal (capa da página) -->
    <h1>Ganhe desconto comprando pela nossa loja virtual. Academia WandersonFit LTDA</h1>

    <!-- Caixa de texto para a segunda frase -->
    <div class="text-box">
        <p class="sub-title">Acesse aqui a nossa loja de cosméticos venha ficar grandão :</p>
        <button on:click={irParaLoja}>Loja</button>
    </div>
</div>