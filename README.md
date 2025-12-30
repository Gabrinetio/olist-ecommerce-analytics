# 📊 Análise de Vendas do E-commerce Olist

Este projeto apresenta uma Análise Exploratória de Dados (EDA) detalhada sobre o dataset público da **Olist**, a maior loja de departamentos dos marketplaces brasileiros. O objetivo é extrair insights estratégicos sobre o comportamento do consumidor, logística e performance de produtos entre 2016 e 2018.

## 📌 Visão Geral
O notebook `Analise_Vendas_Olist.ipynb` realiza o processamento de dados reais de e-commerce para responder a perguntas de negócio fundamentais:
* **Geografia:** Onde estão concentrados os clientes?
* **Sazonalidade:** Como as vendas evoluem ao longo do tempo?
* **Produtos:** O que está a ser comprado?

## 🛠 Tecnologias Utilizadas
O projeto foi desenvolvido em **Python 3** utilizando as seguintes bibliotecas para manipulação e visualização de dados:

* [Pandas](https://pandas.pydata.org/) - Limpeza, fusão (`merge`) e manipulação de DataFrames.
* [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/) - Criação de gráficos estáticos para análise visual.

## 📂 Estrutura do Projeto

### 1. Notebook Principal
* `Analise_Vendas_Olist.ipynb`: Contém todo o código de carregamento, limpeza e visualização. O fluxo de trabalho inclui:
    * Conexão ao Google Drive para leitura dos dados.
    * Conversão de colunas temporais (`datetime`).
    * Tratamento de valores nulos (pedidos não entregues/cancelados).
    * Criação de um dataset unificado (`df_completo`) através da junção de 4 tabelas relacionais.

### 2. Dados Necessários
O código espera os seguintes ficheiros CSV (disponíveis no [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)):
* `olist_customers_dataset.csv`
* `olist_orders_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_products_dataset.csv`

> **Nota:** No código atual, os dados são carregados a partir do caminho `/content/drive/MyDrive/...`. Se for executar localmente, altere a variável `caminho_dos_arquivos`.

## 🚀 Como Executar

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/Gabrinetio/olist-ecommerce-analytics/olist-ecommerce-analytics.git](https://github.com/Gabrinetio/olist-ecommerce-analytics/olist-ecommerce-analytics.git)
    ```
2.  Instale as dependências:
    ```bash
    pip install pandas matplotlib seaborn
    ```
3.  Certifique-se de que os ficheiros CSV estão na pasta correta ou ajuste o caminho no notebook.
4.  Execute o Jupyter Notebook.

## 📈 Principais Insights
Com base na análise realizada:

* **Concentração Regional:** O estado de **São Paulo (SP)** concentra mais de **40%** da base de clientes, seguido pelos restantes estados da região Sudeste (RJ, MG). Isso indica uma forte dependência logística nesta região.
* **Evolução Temporal:** Existe uma tendência de crescimento no volume de pedidos ao longo do período analisado (2016-2018), com picos de vendas visíveis em períodos específicos.

## ✒️ Autor
**Gabriel Santana** Data: 09 de setembro de 2025

---
*Este projeto foi desenvolvido para fins educacionais e de portfólio na área de Ciência de Dados.*
