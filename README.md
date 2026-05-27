# projeto-agro  

projeto do agrinho
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto Agrinho 2026 - Inovação e Sustentabilidade</title>
    
    <!-- ESTILO VISUAL (CSS) -->
    <style>
        :root {
            --verde-principal: #2e7d32;
            --verde-claro: #e8f5e9;
            --verde-escuro: #1b5e20;
            --cinza-texto: #333333;
            --alerta: #c62828;
            --sucesso: #2e7d32;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9fbf7;
            color: var(--cinza-texto);
            line-height: 1.6;
        }

        header {
            background-color: var(--verde-principal);
            color: white;
            text-align: center;
            padding: 2.5rem 1rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header h1 {
            margin: 0;
            font-size: 2.2rem;
        }

        header p {
            margin: 0.5rem 0 0 0;
            font-size: 1.1rem;
            opacity: 0.9;
        }

        .container {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .card {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            margin-bottom: 2rem;
            border: 1px solid #e0e0e0;
        }

        h2 {
            color: var(--verde-escuro);
            margin-top: 0;
            border-bottom: 2px solid var(--verde-claro);
            padding-bottom: 0.5rem;
        }

        /* PAINEL DE METRICAS */
        .painel-sensores {
            display: flex;
            justify-content: space-between;
            gap: 1rem;
            margin: 2rem 0;
        }

        .bloco-sensor {
            flex: 1;
            text-align: center;
            padding: 1.5rem;
            background-color: var(--verde-claro);
            border-radius: 8px;
            transition: transform 0.2s;
        }

        .bloco-sensor:hover {
            transform: translateY(-3px);
        }

        .bloco-sensor h3 {
            margin: 0;
            font-size: 1.1rem;
            color: var(--verde-escuro);
        }

        .bloco-sensor .valor {
            font-size: 2rem;
            font-weight: bold;
            margin: 0.5rem 0;
            color: #111;
        }

        .status-alerta {
            color: var(--alerta) !important;
        }

        .status-sucesso {
            color: var(--sucesso) !important;
        }

        /* BOTÃO */
        .btn-atualizar {
            background-color: var(--verde-principal);
            color: white;
            border: none;
            padding: 0.8rem 2rem;
            font-size: 1rem;
            font-weight: bold;
            border-radius: 6px;
            cursor: pointer;
            display: block;
            margin: 0 auto;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        .btn-atualizar:hover {
            background-color: var(--verde-escuro);
        }

        /* INTEGRANTES */
        .lista-integrantes {
            list-style: none;
            padding: 0;
        }

        .lista-integrantes li {
            padding: 0.5rem 0;
            border-bottom: 1px dashed #ddd;
        }

        footer {
            text-align: center;
            padding: 2rem;
            color: #666;
            font-size: 0.9rem;
            background-color: #f1f1f1;
            margin-top: 4rem;
        }

        /* RESPONSIVIDADE */
        @media (max-width: 600px) {
            .painel-sensores {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <!-- CABEÇALHO DO PROJETO -->
    <header>
        <h1>Agrinho 2026: Sustentabilidade Digital</h1>
        <p>Tecnologia IoT Aplicada à Agricultura Familiar - 1º Ano Ensino Médio</p>
    </header>

    <div class="container">

        <!-- SESSÃO 1: DASHBOARD INTERATIVO -->
        <section class="card">
            <h2>Monitoramento em Tempo Real (Simulação)</h2>
            <p>Clique no botão abaixo para simular a leitura dos dados capturados pelos sensores de campo da nossa horta experimental.</p>
            
            <div class="painel-sensores">
                <div class="bloco-sensor">
                    <h3>Umidade do Solo</h3>
                    <div id="txt-umidade" class="valor">--%</div>
                </div>
                <div class="bloco-sensor">
                    <h3>Temperatura do Ar</h3>
                    <div id="txt-temp" class="valor">--°C</div>
                </div>
                <div class="bloco-sensor">
                    <h3>Status do Sistema</h3>
                    <div id="txt-status" class="valor" style="font-size: 1.4rem;">Aguardando</div>
                </div>
            </div>

            <button class="btn-atualizar" onclick="simularLeituraSensores()">Atualizar Sensores</button>
        </section>

        <!-- SESSÃO 2: DOCUMENTAÇÃO DO PROJETO -->
        <section class="card">
            <h2>Sobre a Nossa Ideia</h2>
            <p>Este site representa o protótipo de uma plataforma de monitoramento agrícola. O objetivo do grupo é combater o desperdício de água e prever pragas causadas pelo excesso de umidade no solo.</p>
            <p>Utilizando o conceito de Internet das Coisas (IoT), pequenos produtores rurais da nossa comunidade podem saber exatamente a hora de ligar e desligar seus sistemas de irrigação diretamente pelo celular.</p>
        </section>

        <!-- SESSÃO 3: IDENTIFICAÇÃO DA EQUIPE -->
        <section class="card">
            <h2>Equipe de Desenvolvimento</h2>
            <ul class="lista-integrantes">
                <li><strong>Estudantes:</strong> Integrante 1, Integrante 2, Integrante 3 e Integrante 4</li>
                <li><strong>Professor(a) Orientador(a):</strong> Nome do Professor</li>
                <li><strong>Colégio:</strong> Seu Colégio Estadual - 1º Ano do Ensino Médio</li>
            </ul>
        </section>

    </div>

    <!-- RODAPÉ -->
    <footer>
        <p>&copy; 2026 Concurso Agrinho - Paraná. Todos os direitos reservados.</p>
    </footer>

    <!-- LÓGICA DE FUNCIONAMENTO (JAVASCRIPT) -->
    <script>
        function gerarValorAleatorio(min, max) {
            return (Math.random() * (max - min) + min).toFixed(1);
        }

        function simularLeituraSensores() {
            // Simula valores comuns de sensores reais
            const umidade = gerarValorAleatorio(35, 85);
            const temperatura = gerarValorAleatorio(16, 34);
            
            const elementoUmidade = document.getElementById('txt-umidade');
            const elementoTemp = document.getElementById('txt-temp');
            const elementoStatus = document.getElementById('txt-status');

            // Atualiza os textos na tela
            elementoUmidade.innerText = `${umidade}%`;
            elementoTemp.innerText = `${temperatura}°C`;

            // Lógica de alerta baseada nas métricas do campo
            if (umidade < 50) {
                elementoStatus.innerText = "Solo Seco: Irrigar!";
                elementoStatus.className = "valor status-alerta";
            } else if (umidade >= 50 && umidade <= 75) {
                elementoStatus.innerText = "Solo Ideal";
                elementoStatus.className = "valor status-sucesso";
            } else {
                elementoStatus.innerText = "Encharcado!";
                elementoStatus.className = "valor status-alerta";
            }
        }

        // Executa uma primeira leitura automática assim que a página abre
        window.onload = simularLeituraSensores;
    </script>
</body>
</html>

