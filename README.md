<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doko Demo Issyo - Matcha Pastel Blog</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">

    <style>
        :root {
            /* Paleta Verde Pastel Soft & Matcha */
            --pastel-green-main: #B5EAD7;
            --pastel-green-soft: #E2F0CB;
            --pastel-bg-soft: #F2F9F4;
            --pastel-card: #FFFFFF;
            --pastel-text: #2C4A3E;
            --pastel-accent: #457B6D;
            --pastel-border: #C8E6C9;
            --pastel-green-glow: rgba(181, 234, 215, 0.45);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Nunito', 'Segoe UI', sans-serif;
            background-color: var(--pastel-bg-soft);
            color: var(--pastel-text);
            line-height: 1.8;
            padding: 30px 15px;
            background-image: radial-gradient(#C8E6C9 1.5px, transparent 1.5px);
            background-size: 22px 22px;
        }

        .container {
            max-width: 850px;
            margin: 0 auto;
            background-color: var(--pastel-card);
            border-radius: 28px;
            box-shadow: 0 15px 35px var(--pastel-green-glow);
            overflow: hidden;
            border: 2px solid var(--pastel-border);
        }

        /* Header estilo Matcha Soft */
        .header-titulo {
            background: linear-gradient(135deg, #B5EAD7 0%, #E2F0CB 100%);
            color: #1B3B30;
            text-align: center;
            padding: 45px 20px;
            border-bottom: 4px solid #A3DECA;
        }

        .header-titulo h1 {
            font-family: 'Fredoka', cursive;
            font-size: 2.6rem;
            font-weight: 700;
            letter-spacing: 0.5px;
            text-transform: lowercase;
            text-shadow: 2px 2px 0px rgba(255, 255, 255, 0.8);
        }

        .content {
            padding: 35px 25px;
        }

        .autor {
            font-family: 'Fredoka', cursive;
            font-size: 1.15rem;
            color: var(--pastel-accent);
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 12px;
            border-bottom: 2px dashed var(--pastel-border);
        }

        h2 {
            font-family: 'Fredoka', cursive;
            color: var(--pastel-text);
            font-size: 1.6rem;
            margin-top: 30px;
            margin-bottom: 15px;
            text-transform: lowercase;
            display: inline-block;
            background: linear-gradient(180deg, transparent 60%, #E2F0CB 60%);
            padding: 0 8px;
        }

        p {
            font-size: 1.05rem;
            color: var(--pastel-text);
            margin-bottom: 20px;
            text-align: justify;
        }

        /* Seção dos Personagens (Pokepi Cards) */
        .personagens-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 18px;
            margin: 20px 0 30px 0;
        }

        .personagem-card {
            background-color: #F4FBF7;
            border: 2px solid var(--pastel-border);
            border-radius: 18px;
            padding: 20px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .personagem-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 18px var(--pastel-green-glow);
        }

        .personagem-card h3 {
            font-family: 'Fredoka', cursive;
            font-size: 1.3rem;
            color: #1B3B30;
            margin-bottom: 4px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .personagem-card .especie {
            font-size: 0.85rem;
            font-weight: bold;
            color: var(--pastel-accent);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 10px;
            display: block;
        }

        .personagem-card p {
            font-size: 0.95rem;
            margin-bottom: 0;
            text-align: left;
            color: var(--pastel-text);
        }

        /* Cartões dos Jogos Famosos */
        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 18px;
            margin-top: 20px;
        }

        .game-card {
            background-color: #E8F5E9;
            border-left: 5px solid var(--pastel-green-main);
            padding: 18px;
            border-radius: 16px;
            box-shadow: 0 4px 12px rgba(181, 234, 215, 0.2);
        }

        .game-card h3 {
            font-family: 'Fredoka', cursive;
            color: #2D5A4C;
            font-size: 1.15rem;
            margin-bottom: 8px;
        }

        .game-card p {
            font-size: 0.95rem;
            margin-bottom: 0;
            text-align: left;
        }

        footer {
            text-align: center;
            padding: 25px;
            font-size: 0.95rem;
            color: #457B6D;
            background-color: #E8F5E9;
            border-top: 2px solid var(--pastel-border);
            font-family: 'Fredoka', cursive;
        }
    </style>
</head>
<body>

    <div class="container">
        <header class="header-titulo">
            <h1>🌿 Doko Demo Issyo – O jogo que transformou Toro Inoue em uma celebridade. 🌿</h1>
        </header>

        <div class="content">
            <h2>personagens (pokepi)</h2>
            <div class="personagens-grid">
                
                <div class="personagem-card">
                    <h3>🐱 Toro Inoue</h3>
                    <span class="especie">Gato Branco</span>
                    <p>O protagonista ingênuo, otimista e afetuoso. Seu maior sonho é aprender tudo sobre os humanos para um dia se transformar em um ser humano de verdade.</p>
                </div>

                <div class="personagem-card">
                    <h3>😼 Kuro</h3>
                    <span class="especie">Gato Preto</span>
                    <p>O melhor amigo e rival de Toro. É sarcástico, adora tecnologia, bebidas, noitadas e agir como se fosse um cara rebelde e descolado.</p>
                </div>

                <div class="personagem-card">
                    <h3>🐱 Sora</h3>
                    <span class="especie">Gato Mago / Poeta</span>
                    <p>Um gato calmo, romântico e sonhador. Ama natureza, poesia e tem uma personalidade tranquila e meio avoada.</p>
                </div>

                <div class="personagem-card">
                    <h3>🐰 Jun</h3>
                    <span class="especie">Coelho</span>
                    <p>Um coelho extremamente antenado com a cultura pop, moda e idols. É tagarela, super animado e adora ser o centro das atenções.</p>
                </div>

                <div class="personagem-card">
                    <h3>🐩 Pierre</h3>
                    <span class="especie">Cão Poodle</span>
                    <p>Um poodle refinado, elegante e muito sensível. Ama cultura francesa, artes, música e tem um coração puro e gentil.</p>
                </div>

                <div class="personagem-card">
                    <h3>🐸 Ricky</h3>
                    <span class="especie">Sapo</span>
                    <p>Um sapo muito focado em artes marciais e treino físico. Apesar da sua busca por sabedoria e disciplina mental, é engraçado e sincero.</p>
                </div>

            </div>

            <h2>história da franquia</h2>
            <p>
                A franquia <strong>Doko Demo Issyo</strong> foi criada pelo estúdio <strong>Bomber eXpress</strong> (atualmente conhecido como <em>BeXide</em>) em parceria com a Sony Computer Entertainment. O primeiro jogo foi lançado no Japão em 22 de julho de 1999 para o console PlayStation original. A franquia foi projetada especialmente para tirar proveito do <strong>PocketStation</strong> — um periférico de cartão de memória com tela que permitia levar os personagens no bolso. A premissa inovadora envolvia ensinar palavras da vida real para seres virtuais chamados <em>Pokepi</em> ("Pocket People"). O imenso carisma do gato branco <strong>Toro Inoue</strong> fez o jogo se tornar um grande fenômeno de vendas e popularidade, transformando o personagem no mascote oficial da marca PlayStation no Japão.
            </p>

            <h2>jogos famosos</h2>
            <p>
                Ao longo dos anos, a franquia lançou diversos títulos marcantes em diferentes plataformas, mantendo o foco em interatividade, simulação de vida e humor leve:
            </p>

            <div class="game-grid">
                <div class="game-card">
                    <h3>Doko Demo Issyo (1999 - PS1 / PSP)</h3>
                    <p>O jogo clássico onde você conversa e ensina vocabulário para seu Pokepi, podendo levá-lo no PocketStation para interagir em qualquer lugar.</p>
                </div>
                <div class="game-card">
                    <h3>Toro to Kyuujitsu (2001 - PS2)</h3>
                    <p>Um jogo inovador de simulação onde Toro passeia por uma cidade japonesa real em vídeo live-action enquanto conversa com o jogador.</p>
                </div>
                <div class="game-card">
                    <h3>Mainichi Issho (2006 - PS3 / PSP)</h3>
                    <p>Um aplicativo interativo onde Toro e seu amigo Kuro apresentavam um programa de notícias diárias sobre games, cultura e entretenimento no PlayStation 3.</p>
                </div>
                <div class="game-card">
                    <h3>Toro and Friends: Onsen Town (2019 - Mobile)</h3>
                    <p>Um divertido jogo de quebra-cabeça do tipo match-3 para celulares, onde você ajuda Toro a reconstruir uma famosa cidade de águas térmicas.</p>
                </div>
            </div>
        </div>

        <footer>
            <p>☘️ Doko Demo Issyo Blog — Criado com carinho por Geovana Leal ☘️</p>
        </footer>
    </div>

</body>
</html>
