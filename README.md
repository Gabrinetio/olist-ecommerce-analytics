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
* [Jupyter Notebook](https://jupyter.org/) - Ambiente de desenvolvimento interativo.

## 📂 Estrutura do Projeto

### 1. Notebook Principal
* `Analise_Vendas_Olist.ipynb`: Contém todo o código de carregamento, limpeza e visualização. O fluxo de trabalho inclui:
    * Configuração flexível para leitura de dados (Local ou Google Drive).
    * Conversão de colunas temporais (`datetime`).
    * Tratamento de valores nulos (pedidos não entregues/cancelados).
    * Criação de um dataset unificado (`df_completo`) através da junção de 4 tabelas relacionais.

### 2. Dados Necessários
O código espera os seguintes ficheiros CSV (disponíveis no [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)):
* `olist_customers_dataset.csv`
* `olist_orders_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_products_dataset.csv`

## 🚀 Como Executar este Projeto

Para rodar a análise na sua máquina local, siga os passos abaixo:

### 1. Clone o repositório
```bash
git clone [https://github.com/Gabrinetio/olist-ecommerce-analytics.git](https://github.com/Gabrinetio/olist-ecommerce-analytics.git)
cd olist-ecommerce-analytics

```

### 2. Configuração dos Dados (Importante!)

Os dados originais não estão incluídos no repositório para economizar espaço. Siga esta estrutura:

1. Baixe o dataset oficial no Kaggle: [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).
2. Crie uma pasta chamada `data` na raiz do projeto.
3. Extraia todos os arquivos `.csv` para dentro desta pasta.

A estrutura de arquivos deve ficar assim:

```text
olist-ecommerce-analytics/
├── data/                       <-- Pasta criada por você com os CSVs
│   ├── olist_customers_dataset.csv
│   └── ...
├── Analise_Vendas_Olist.ipynb
├── requirements.txt
└── README.md

```

### 3. Instalação das Dependências

Instale as bibliotecas necessárias listadas no arquivo `requirements.txt`:

```bash
pip install -r requirements.txt

```

### 4. Executando o Notebook

Abra o arquivo `Analise_Vendas_Olist.ipynb` no seu editor favorito (VS Code, Jupyter Notebook ou Jupyter Lab) e execute as células.

> **Nota:** O notebook está configurado para buscar os arquivos automaticamente na pasta `data/`.

## 📈 Principais Insights

Com base na análise realizada:

* **Concentração Regional:** O estado de **São Paulo (SP)** concentra mais de **40%** da base de clientes, seguido pelos restantes estados da região Sudeste (RJ, MG). Isso indica uma forte dependência logística nesta região.
* **Evolução Temporal:** Existe uma tendência de crescimento no volume de pedidos ao longo do período analisado (2016-2018), com picos de vendas visíveis em períodos específicos.

## ✒️ Autor

**Gabriel Santana**

---

*Este projeto foi desenvolvido para fins educacionais e de portfólio na área de Ciência de Dados.*

```
