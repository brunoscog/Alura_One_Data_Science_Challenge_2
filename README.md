<p align="center">
  <img src="brunoscog-cover.jpg" alt="Imagem de capa do projeto">
</p>

<h1 align="center"> ONE | Alura - Challenge 2: Análise de Evasão de Clientes (Churn) </h1>

<p align="center">
  <img src="http://img.shields.io/static/v1?label=STATUS&message=PROJETO%20CONCLUÍDO&color=GREEN&style=for-the-badge"/>
  <br>
  <img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-20232A?style=for-the-badge&logo=matplotlib&logoColor=white" />
  <img src="https://img.shields.io/badge/seaborn-20232A?style=for-the-badge&logo=seaborn&logoColor=white" />
</p>

# 📌 Índice

* [Descrição do Projeto](#descrição-do-projeto)
* [Funcionalidades](#funcionalidades)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Como Executar](#como-executar)
* [Estrutura do Projeto](#estrutura-do-projeto)
* [Resultado da Análise](#resultado-da-análise)
* [Acesse o projeto completo](#acesse-o-projeto-completo)
* [Desenvolvido por](#desenvolvido-por)

## 🧾 Descrição do Projeto

Este projeto aborda o desafio de **análise de evasão de clientes (Churn)** da **Telecom X**, uma empresa de telecomunicações. O objetivo principal é identificar os fatores que levam os clientes a cancelar seus serviços, fornecendo insights para que a equipe de Data Science possa desenvolver estratégias de retenção mais eficazes e modelos preditivos.

O trabalho envolveu um processo completo de **ETL (Extração, Transformação e Carga)** dos dados, seguido por uma **Análise Exploratória de Dados (EDA)** detalhada, com foco na visualização e interpretação de padrões que impactam a decisão de permanência ou saída do cliente.

---

## ✅ Funcionalidades

-   **Extração de Dados:** Coleta de dados de clientes diretamente de uma API externa (formato JSON).
-   **Limpeza e Tratamento (ETL):** Normalização de dados aninhados, tratamento de inconsistências (valores ausentes, strings vazias) e padronização de variáveis.
-   **Criação de Novas Métricas:** Desenvolvimento de colunas como o "Gasto Diário" para análises mais granulares.
-   **Análise Descritiva:** Geração de estatísticas para compreender a distribuição e comportamento dos dados.
-   **Visualização de Dados Estratégica:** Criação de gráficos padronizados para identificar padrões de evasão por:
    * Distribuição geral do Churn.
    * Variáveis demográficas (Gênero, Idosos, Parceiros, Dependentes).
    * Tipo de contrato e forma de pagamento.
    * Variáveis numéricas (Tempo de contrato, Gasto Total, Gasto Diário).
-   **Análise de Correlação:** Quantificação da relação linear entre as variáveis numéricas e a evasão.
-   **Relatório Final:** Consolidação de todo o trabalho, com conclusões, insights e recomendações práticas para a Telecom X.

---

## 💻 Tecnologias Utilizadas

-   Python 3.x
-   pandas
-   matplotlib
-   seaborn
-   Google Colab / Jupyter Notebook

---

## ▶️ Como Executar

```bash
# Clone o repositório (substitua 'seu_usuario' pelo seu nome de usuário no GitHub)
git clone [https://github.com/seu_usuario/nome_do_seu_repositorio.git](https://github.com/seu_usuario/nome_do_seu_repositorio.git)
cd nome_do_seu_repositorio

# Instale as bibliotecas necessárias
pip install pandas matplotlib seaborn requests

# Abra o notebook
```
Abra o arquivo Challege 2 - TelecomX.ipynb no Jupyter Notebook ou Google Colab.
Nota: Os dados serão carregados diretamente de uma URL do GitHub, portanto, não há necessidade de baixar arquivos CSV adicionais.

## 📁 Estrutura do Projeto

```bash
├── Challege 2 - TelecomX.ipynb  # Notebook principal com a análise, gráficos e relatório
├── README.md                    # Documentação do projeto
├── brunoscog-cover.jpg          # Imagem de capa (opcional, adicione se tiver uma)
```
---

## 📊 Resultado da Análise
A análise revelou insights cruciais sobre a evasão de clientes:

* 📉 **Fatores de Maior Evasão (Churn)**:

  *  **Contratos Mês a Mês** (`Month-to-month`): Clientes com este tipo de contrato apresentam a maior taxa de churn.
  *  **Forma de Pagamento Electronic check**: Associada a uma proporção significativamente maior de evasão.
  *  **Contas Mensais Elevadas** (`account_Charges.Monthly`): Clientes com gastos mensais mais altos mostram maior tendência a sair.
  *  **Fatura Online** (`account_PaperlessBilling`): Clientes que recebem fatura online também tendem a evadir mais.
  *  **Clientes Idosos** (`SeniorCitizen`): Apresentam uma leve tendência de maior churn.
* 📈 **Fatores de Retenção (Menor Churn)**:
  *  **Tempo de Contrato** (`customer_tenure`): Aumenta significativamente a lealdade do cliente; quanto maior o tempo de serviço, menor a chance de evasão.
  *  **Serviços de Segurança e Suporte** (`internet_OnlineSecurity`, `internet_TechSupport`): Clientes que assinam esses serviços adicionais têm menor probabilidade de cancelar.
  *  **Situação Familiar** (`customer_Partner`, `customer_Dependents`): Clientes com parceiro(a) ou dependentes tendem a ser mais estáveis e menos propensos a sair.
  *  **Gasto Total Acumulado** (`account_Charges.Total`): Clientes com maior gasto total ao longo do tempo são mais leais.

##📝 **Recomendações Principais**: Foco em programas de engajamento para novos clientes e aqueles com contratos mensais, incentivo à adesão de serviços de segurança e suporte, e investigação e melhoria da experiência com o método de pagamento 'Electronic check'.

---

## 📘 Acesse o projeto completo

O notebook com toda a análise, gráficos e relatório final está disponível em:

👉 [`Challege 2 - TelecomX.ipynb`](./Challege%202%20-%20TelecomX.ipynb)

---

## 👨‍💻 Desenvolvido por

<img src="https://media.licdn.com/dms/image/v2/D4D03AQE5oHHVZzjwIg/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1727484820568?e=2147483647&v=beta&t=JuBlRoJK5c2EUbs18LthUHalzmlM4A_2Zi16PzAlwmc" width=115>
