🌡️ Monitor de Temperaturas Systemp (CCO | Malha Sul)

Um dashboard interativo e responsivo desenvolvido para o monitoramento de temperaturas e condições climáticas de diferentes malhas ferroviárias. O sistema foi projetado para auxiliar o Centro de Controle Operacional (CCO) na tomada de decisões, emitindo alertas visuais para condições extremas que possam impactar a operação.

🚀 Versões do Projeto
Este repositório contém duas versões do sistema, criadas para diferentes propósitos de demonstração e uso:

temperaturas.html (Versão de Produção/API): 
Consome dados meteorológicos reais utilizando a API Open-Meteo. Traz a previsão do tempo para as próximas 72 horas com base em modelos globais oficiais.

simulador-inverno.html (Versão de Simulação):
Uma versão offline que possui um motor interno (mock) gerador de dados térmicos. Ele simula cenários específicos de inverno (frio extremo, geadas e variações de temperatura) para testes de interface e demonstração de alertas.

✨ Funcionalidades Principais
Navegação por Malhas: Separação das estações por regiões (Rio Grande, São Francisco, Oeste PR, Central e CTC).

Previsão de 72 Horas: Controle de visualização por dias (Hoje, D+1, D+2) e um slider intuitivo de horário (intervalos de 2 horas).

Sistema de Alertas Dinâmicos: Cards que mudam de cor e emitem alertas baseados nas condições climáticas:

❄️ Frio Extremo / Geada: Temperaturas abaixo de 5ºC.

⚠️ Calor (Risco de Interdição): Temperaturas acima de 29ºC.

🌩️ Tempestade: Detecção de chuva severa.

Gráficos Evolutivos: Ao clicar em um card, um modal exibe um gráfico de linha detalhado com a curva térmica de 24 horas, destacando as faixas de risco (calor/frio) e períodos de chuva.

Exportação em PDF: Geração automática de relatórios compactados da tela atual para facilitar o arquivamento e compartilhamento de dados.

Design Responsivo: Interface limpa, moderna e adaptada para dispositivos móveis, incluindo um menu lateral (hambúrguer) para telas menores.

🛠️ Tecnologias Utilizadas
HTML5, CSS3 e JavaScript (Vanilla): Estrutura, estilo e lógica de interface.

Chart.js: Renderização dos gráficos dinâmicos de temperatura.

Chart.js Plugin Annotation: Desenho das faixas de risco e zonas de chuva dentro dos gráficos.

html2pdf.js: Motor de conversão da interface web para documentos PDF.

Open-Meteo API: Fornecimento de dados meteorológicos reais e gratuitos (utilizado no arquivo temperaturas.html).

💻 Como Executar
O projeto é puramente Front-end e não requer instalação de pacotes (Node.js, npm, etc) ou configuração de banco de dados.

Faça o clone deste repositório:

Bash
git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
Navegue até a pasta do projeto.

Abra o arquivo temperaturas.html ou simulador-inverno.html diretamente em qualquer navegador web moderno (Chrome, Edge, Firefox, Safari).

Desenvolvido por Ewerton Siqueira Medeiros
