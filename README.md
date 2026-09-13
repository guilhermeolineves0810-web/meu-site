<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Meu Primeiro Site</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #f4f4f4;
            color: #222;
        }

        header {
            background: #111;
            color: white;
            padding: 20px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 24px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 25px;
        }

        nav a:hover {
            color: #00aaff;
        }

        .hero {
            min-height: 500px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(135deg, #111, #333);
            color: white;
        }

        .hero h2 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 20px;
            color: #ccc;
            margin-bottom: 30px;
        }

        .botao {
            display: inline-block;
            background: #00aaff;
            color: white;
            padding: 14px 30px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
            border: none;
        }

        .botao:hover {
            background: #0088cc;
        }

        section {
            padding: 70px 8%;
        }

        section h2 {
            text-align: center;
            margin-bottom: 40px;
            font-size: 32px;
        }

        .cards {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
        }

        .card {
            background: white;
            width: 300px;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            text-align: center;
        }

        .card h3 {
            margin-bottom: 15px;
        }

        .card p {
            color: #666;
            line-height: 1.6;
        }

        footer {
            background: #111;
            color: #aaa;
            text-align: center;
            padding: 25px;
        }

        /* Celular */
        @media (max-width: 600px) {

            header {
                flex-direction: column;
                gap: 15px;
            }

            nav a {
                margin: 0 8px;
            }

            .hero h2 {
                font-size: 36px;
            }

            .hero p {
                font-size: 17px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>Meu Site</h1>

        <nav>
            <a href="#inicio">Início</a>
            <a href="#sobre">Sobre</a>
            <a href="#projetos">Projetos</a>
        </nav>
    </header>


    <main>

        <section class="hero" id="inicio">

            <div>
                <h2>Olá, mundo! 👋</h2>

                <p>
                    Esse é meu primeiro site hospedado pelo GitHub Pages.
                </p>

                <button class="botao" onclick="mostrarMensagem()">
                    Clique aqui
                </button>
            </div>

        </section>


        <section id="sobre">

            <h2>Sobre o site</h2>

            <div class="cards">

                <div class="card">
                    <h3>HTML</h3>

                    <p>
                        Estrutura da página, textos, botões,
                        imagens e elementos.
                    </p>
                </div>


                <div class="card">
                    <h3>CSS</h3>

                    <p>
                        Responsável pelo visual, cores,
                        espaçamento e responsividade.
                    </p>
                </div>


                <div class="card">
                    <h3>JavaScript</h3>

                    <p>
                        Adiciona interatividade e permite
                        que os elementos respondam ao usuário.
                    </p>
                </div>

            </div>

        </section>


        <section id="projetos">

            <h2>Projetos</h2>

            <div class="cards">

                <div class="card">
                    <h3>Projeto 01</h3>

                    <p>
                        Meu primeiro projeto utilizando HTML e CSS.
                    </p>

                    <br>

                    <button class="botao" onclick="alert('Projeto 01 funcionando!')">
                        Testar
                    </button>
                </div>


                <div class="card">
                    <h3>Projeto 02</h3>

                    <p>
                        Um projeto futuro para colocar aqui.
                    </p>

                    <br>

                    <button class="botao" onclick="alert('Projeto 02 funcionando!')">
                        Testar
                    </button>
                </div>

            </div>

        </section>

    </main>


    <footer>
        <p>© 2026 - Meu Primeiro Site</p>
    </footer>


    <script>

        function mostrarMensagem() {
            alert("Funcionou! 🚀 Seu JavaScript está funcionando.");
        }

    </script>

</body>
</html>
