# Projeto de Análise de IPCA para o Banco IP2CA

Este repositório contém os arquivos para a análise do IPCA, implementando um pipeline de dados desde a extração até a visualização

## Arquitetura da Solução

- **Engenharia de Dados:** Databricks
- **Linguagem:** PySpark e SQL
- **Governança:** Unity Catalog
- **Visualização:** Power BI

## Estrutura do Repositório

- **/databricks_notebooks**: Contém os notebooks para setup da infraestrutura e execução do pipeline de ETL
- **/powerbi_report**: Contém o arquivo `.pbix` do dashboard final.

## Como Executar

1.  **Setup do Ambiente Databricks (Executar 1 vez):**
    - Importe e execute o notebook `setup_catalog` para criar o catálogo e os schemas no Unity Catalog

2.  **Execução do Pipeline:**
    - Importe e execute o notebook `pipeline-ipca` para processar os dados e popular as tabelas da camada Gold

3.  **Visualização:**
    - Abra o arquivo `ANÁLISE IPCA.pbix` e atualize a conexão com as credenciais do seu ambiente Databricks para visualizar os dados

## Processo de criação

- Identidade visual criada do zero visando cores impactantes e que faça sentido com o contexto de BANCO. Relatório possui capa e navegação própria ao invés da nativa, focando em sempre ter atenção nos DADOS, porém sem deixar a parte bonita (UI/UX) de lado

- A base contém 2 colunas principais: DATA | VALOR, dito isso tive que pensar em insights que possam ser de algum avalia para o usuário final, sem grande contexto