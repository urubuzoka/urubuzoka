<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>História do Futebol</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }
        .header {
            background: linear-gradient(to bottom, #9be56a, #3b7a26);
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        h1 {
            margin-top: 0;
        }
        .image-container {
            display: inline-block;
            margin: 20px;
            cursor: pointer;
            transition: transform 0.3s;
        }
        .image-container:hover {
            transform: scale(1.1);
        }
        .image-container img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 10px;
        }
        h2 {
            color: #3b7a26;
            margin-top: 30px;
        }
        ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        li {
            margin-bottom: 10px;
        }
        strong {
            color: #9be56a;
        }
        p {
            line-height: 1.6;
            color: #666;
        }
        .player-info {
            display: none;
            margin-top: 20px;
        }
        .player-info.active {
            display: block;
        }
        .player-caption {
            font-style: italic;
            color: #999;
        }
    </style>
    <script>
        function showPlayerInfo(playerId) {
            // Hide all player-info divs
            var playerInfos = document.querySelectorAll('.player-info');
            playerInfos.forEach(function(info) {
                info.classList.remove('active');
            });

            // Show the selected player-info div
            var playerInfo = document.getElementById(playerId);
            if (playerInfo) {
                playerInfo.classList.add('active');
            }
        }
    </script>
</head>
<body>
    <div class="header">
        <h1>História do Futebol</h1>
    </div>
   
    <div class="container">
        <div class="image-container" onclick="showPlayerInfo('pele-info')">
            <img src="pele.jpg" alt="Pelé">
            <p class="player-caption">Pelé - Rei do Futebol</p>
        </div>
        <div class="image-container" onclick="showPlayerInfo('messi-info')">
            <img src="messi.jpg" alt="Messi">
            <p class="player-caption">Messi - Mais Bolas de Ouro</p>
        </div>
        <div class="image-container" onclick="showPlayerInfo('ronaldo-info')">
            <img src="ronaldo.jpg" alt="Cristiano Ronaldo">
            <p class="player-caption">Cristiano Ronaldo - Mais Influente</p>
        </div>
       
        <div id="pele-info" class="player-info">
            <h2>Pelé</h2>
            <ul>
                <li><strong>Data de Nascimento:</strong> 23 de outubro de 1940</li>
                <li><strong>Gols na Carreira:</strong> Mais de 1200</li>
                <li><strong>Times Jogados:</strong> Santos FC, New York Cosmos</li>
                <li><strong>Clube que torce:</strong> Santos FC</li>
                <li><strong>Títulos:</strong> 3 Copas do Mundo, 10 Campeonatos Paulistas, 2 Copas Libertadores, entre outros.</li>
            </ul>
        </div>
       
        <div id="messi-info" class="player-info">
            <h2>Messi</h2>
            <ul>
                <li><strong>Data de Nascimento:</strong> 24 de junho de 1987</li>
                <li><strong>Gols na Carreira:</strong> Mais de 700</li>
                <li><strong>Times Jogados:</strong> Barcelona, Paris Saint-Germain</li>
                <li><strong>Clube que torce:</strong> Newell's Old Boys</li>
                <li><strong>Títulos:</strong> 7 Bolas de Ouro, 10 La Liga, 4 Champions League, entre outros.</li>
            </ul>
        </div>
       
        <div id="ronaldo-info" class="player-info">
            <h2>Cristiano Ronaldo</h2>
            <ul>
                <li><strong>Data de Nascimento:</strong> 5 de fevereiro de 1985</li>
                <li><strong>Gols na Carreira:</strong> Mais de 800</li>
                <li><strong>Times Jogados:</strong> Sporting CP, Manchester United, Real Madrid, Juventus</li>
                <li><strong>Clube que torce:</strong> Grêmio Foot-Ball Porto Alegrense</li>
                <li><strong>Títulos:</strong> 5 Bolas de Ouro, 7 Ligas Nacionais, 5 Champions League, entre outros.</li>
            </ul>
        </div>
       
        <h2>Origem do Futebol</h2>
        <p>O futebol moderno teve origem na Inglaterra, no século XIX. O esporte evoluiu a partir de jogos antigos que eram praticados em várias partes do mundo. A primeira regra oficial do futebol foi criada em 1863, com a fundação da Football Association (FA) na Inglaterra.</p>
       
        <h2>Sobre o Futebol no Brasil</h2>
        <p>O futebol é o esporte mais popular no Brasil. Introduzido no país por imigrantes britânicos no final do século XIX, o futebol rapidamente se tornou uma paixão nacional. O Brasil é conhecido por sua rica história no esporte, produzindo alguns dos maiores jogadores de todos os tempos, como Pelé, Zico, Romário, Ronaldo e Ronaldinho Gaúcho.</p>
       
        <h2>Resumo</h2>
        <p>O futebol é um esporte apaixonante que une milhões de pessoas ao redor do mundo. Com sua história rica e diversificada, o futebol transcende fronteiras e culturas, proporcionando momentos inesquecíveis tanto para os jogadores quanto para os fãs.</p>
    </div>
</body>
</html>
