# 🎬 Movies Analytics — Pipeline de Dados End-to-End & Dashboard Executivo

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Google BigQuery](https://img.shields.io/badge/Google_BigQuery-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

> 🇧🇷 **PT:** Projeto de dados *End-to-End*: extração, limpeza e manipulação programática via **Python & Pandas (Google Colab)**, armazenamento e consultas de alto desempenho no **Google BigQuery** (.parquet), modelagem e transformação no **Power Query/DAX** e construção de dashboard executivo interativo de 2 páginas no **Power BI** (+33k filmes IMDb/TMDB).  
> 🇺🇸 **EN:** *End-to-End* data pipeline: extraction, cleaning, and manipulation using **Python & Pandas (Google Colab)**, high-performance storage and querying in **Google BigQuery** (.parquet), modeling/transformation via **Power Query/DAX**, and a 2-page executive **Power BI** dashboard (33k+ IMDb/TMDB movies).

---

## 🏗️ Arquitetura do Pipeline de Dados (ETL)

O projeto engloba todo o ciclo de vida dos dados, desde a extração programática em Python até a entrega de inteligência de negócios para tomada de decisão:

```text
[Google Colab: Python + Pandas] ➔ [Google BigQuery: .parquet] ➔ [Power Query / ETL] ➔ [Modelagem DAX] ➔ [Power BI Dashboard]
Extract & Ingestion (Ingestão Programática):

Coleta e manipulação do dataset com +33 mil produções cinematográficas (dados combinados do IMDb e TMDB).

Limpeza inicial, tratamento de nulos e estruturação de colunas utilizando scripts em Python e a biblioteca Pandas no Google Colab.

Data Warehouse & Storage (Armazenamento Colunar):

Carga dos dados processados no Google BigQuery em formato colunar altamente otimizado (Parquet).

Execução de consultas SQL de alta performance para otimização da volumetria e consumo no BI.

Transform & Modeling (Transformação e Regras de Negócio):

Conexão e higienização complementar de tipos e dados no Power Query.

Criação de tabelas, medidas de agregação (AVERAGE, SUM, COUNT) e colunas calculadas condicionais (IF) utilizando a linguagem DAX.

Load & Visualization (Interface Executiva):

Desenvolvimento de modelo relacional e design de UI/UX focado em clareza, padrão visual executivo (tons de bege e castanho) e navegação interativa em tempo real.

📊 Estrutura e Visuais do Dashboard
📄 Página 1: Métricas Gerais
Focada em apresentar o panorama macro e indicadores-chave de desempenho do acervo cinematográfico.

Cartões de KPI Executivos:

Total de Filmes: Quantidade consolidada de títulos no catálogo (+33 mil).

Orçamento Médio: Média financeira investida nas produções.

Nota Média IMDb: Avaliação geral média dos usuários.

Evolução Temporal de Lançamentos:

Gráfico de área demonstrando o volume histórico de produções ao longo dos anos.

Top 5 Melhores Notas IMDb:

Tabela dinâmica com os 5 filmes com maior pontuação.

Regra de Negócio/Filtro de Relevância: Aplicação de regra com filtro mínimo de +1.000 votos para evitar distorções de amostras pequenas.

Filtros e Segmentadores Interativos:

Filtro deslizante por período/anos de lançamento e menu de seleção por género.

📄 Página 2: Análise Detalhada (Óscares & Prestígio)
Focada em mensurar o impacto do prémio Óscar na avaliação do público e no perfil do catálogo.

KPI de Premiações:

Qtd. Total de Óscares: Indicador numérico das estatuetas acumuladas pelas produções do catálogo.

Impacto na Avaliação (Com vs. Sem Óscar):

Gráfico de colunas agrupadas comparando a Nota Média do IMDb entre filmes vencedores de estatuetas (Com Óscar) e não premiados (Sem Óscar), evidenciando o acréscimo de nota em produções premiadas.

Top Filmes Vencedores:

Tabela com o ranking dos títulos que conquistaram o maior número de premiações na história do cinema.

Óscares por Género:

Gráfico de barras horizontais indicando a distribuição das estatuetas entre as categorias de filmes (ex: Drama, Comédia, Period Drama, etc.).

Segmentador por Intervalo de Anos:

Barra deslizante (Slider) para exploração temporal dinâmica da premiação.

🛠️ Tecnologias e Conceitos Aplicados
Python & Pandas (Google Colab): Engenharia e pré-processamento de dados programático.

Google BigQuery & Parquet: Data Warehouse em nuvem com formato colunar otimizado para consultas analíticas rápidas.

Power Query (M): Limpeza, ajuste de schema, criação de colunas e tipagem no Power BI.

Linguagem DAX:

Métricas agregadas de contagem, soma e média.

Lógica condicional para categorização de filmes premiados vs. não premiados.

UI/UX & Design Executivo: Princípios de Design de Dashboards, hierarquia visual, paleta corporativa sobriedade (bege e castanho) e cartões de métricas destacados.

Filtragem Avançada: Combinação de filtros Top N com métricas de volume (mínimo de avaliações).

📂 Como Reproduzir e Utilizar este Repositório
Clonar o Repositório:

Bash
git clone [https://github.com/Lopess01/powerbi-movies-analytics.git](https://github.com/Lopess01/powerbi-movies-analytics.git)
Abrir o Relatório:

Certifica-te de ter o Power BI Desktop instalado.

Abre o ficheiro Movies_Analytics.pbix.

Explorar a Análise:

Navega entre as páginas Métricas Gerais e Análise Detalhada.

Utiliza os segmentadores de dados para filtrar perfeitamente por período ou género.

📄 Licença
Este projeto está sob a licença MIT - sinta-se à vontade para utilizar e adaptar.
