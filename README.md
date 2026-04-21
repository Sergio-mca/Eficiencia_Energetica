⚡ Análise de Eficiência Energética com Dados da ANEEL
🚀 Visão Geral

Este projeto tem como objetivo analisar a eficiência da geração de energia no Brasil utilizando dados públicos da ANEEL.

Através de processamento distribuído com PySpark, realizo o tratamento, enriquecimento e agregação dos dados para gerar métricas estratégicas que podem apoiar análises operacionais e decisões no setor elétrico.

🎯 Problema de Negócio

Como medir e acompanhar a eficiência da geração de energia considerando diferentes estados, tipos de geração e períodos ao longo do tempo?

🧠 Fonte de Dados
Origem: ANEEL (Agência Nacional de Energia Elétrica)
Dados utilizados:
Empreendimentos de geração
Potência outorgada
Potência fiscalizada
Garantia física
Datas operacionais
🛠️ Tecnologias Utilizadas
PySpark → processamento de grandes volumes de dados
Python → manipulação e lógica
Google Colab → ambiente de execução
CSV (ANEEL) → fonte de dados
Looker Studio (destino) → visualização futura
⚙️ Pipeline de Dados
🔹 1. Ingestão

Leitura de múltiplos arquivos CSV contendo dados de geração de energia.

🔹 2. Tratamento
Padronização de colunas
Limpeza de espaços e formatação
Conversão de tipos (string → numérico/data)
Ajuste de separadores decimais
🔹 3. Enriquecimento

Criação de novas variáveis:

Ano e mês
Eficiência de geração (%)

📌 Fórmula de eficiência:

Eficiência (%) = Potência Fiscalizada / Potência Outorgada * 100
🔹 4. Agregação

Os dados são agrupados por:

Ano
Mês
Estado (UF)
Tipo de geração

Gerando métricas como:

Número de empreendimentos
Potência média (outorgada e fiscalizada)
Eficiência média
Potência total
🔹 5. Exportação

Os dados tratados são exportados para CSV, prontos para uso em ferramentas de BI como o Looker Studio.

📊 Principais Insights (Potenciais)
Diferenças de eficiência entre tipos de geração (hidrelétrica, eólica, etc.)
Variações regionais de desempenho energético
Evolução temporal da eficiência
Identificação de possíveis ineficiências operacionais
💡 Diferenciais do Projeto

✔ Uso de PySpark (escalabilidade real de dados)
✔ Pipeline completo: ingestão → tratamento → análise → saída
✔ Foco em métrica de negócio (eficiência)
✔ Preparado para integração com BI

📁 Estrutura do Projeto
📦 Eficiencia_Energetica
 ┣ 📜 dados_eficiencia_geracao.py
 ┣ 📄 README.md
 ┗ 📊 dados_tratados.csv (gerado)
▶️ Como Executar
1. Instalar dependências
pip install pyspark
2. Executar o script / notebook
Pode ser rodado no Google Colab ou ambiente local
Ajuste os caminhos dos arquivos CSV
3. Resultado

Um arquivo final será gerado:

energia_tratada_aneel.csv
📈 Próximos Passos (Evolução do Projeto)
Criar dashboard no Power BI ou Looker Studio
Adicionar análise preditiva (forecast de eficiência)
Criar indicadores de performance (KPIs energéticos)
Automatizar pipeline com Airflow ou similar
👨‍💻 Sobre mim

Profissional em transição para a área de Dados, com foco em:

Análise de dados
BI (Power BI)
Engenharia de dados (PySpark)

Buscando aplicar dados para gerar impacto real no negócio.

📬 Contato

Aberto a oportunidades em Dados 🚀
