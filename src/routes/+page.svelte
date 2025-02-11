<script>
    function irParaLoja() {
        window.location.href = "/https://wanwansite.github.io/loja";
    }

    function irParaFrases() {
        window.location.href = "https://wanwansite.github.io/frases";
    }
</script>

<svelte:head>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            height: 100%;
        }

        .fundodosite {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            padding-top: 80px;
            background-color: #263238;
        }

        h1 {
            font-size: 50px;
            font-weight: 700;
            text-align: center;
            color: #fff;
            margin-top: 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }

        .text-box {
            background-color: rgb(255, 255, 255);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 80%;
            max-width: 600px;
            text-align: center;
        }

        .sub-title {
            font-size: 24px;
            font-weight: 600;
            color: #333;
            margin-bottom: 20px;
        }

        button {
            background-color: rgb(221, 123, 67);
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
            background-color: rgb(255, 94, 0);
        }
    </style>
</svelte:head>

<div class="fundodosite">
    <h1>compre pela nossa loja virtual. Academia WandersonFit LTDA</h1>
    <div class="text-box">
        <p class="sub-title">Acesse aqui a nossa loja de cosméticos venha ficar GIGANTE :</p>
        <button on:click={irParaLoja}>Loja</button>
        <p class="sub-title">Está se sentindo desmotivado para ir treinar? Conheça nossa página que te dá motivos para não perder um dia de treino!</p>
        <button class="btn btn-primary" on:click={irParaFrases}>Frases</button>
    </div>
</div>
