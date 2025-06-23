# RFM_Clusters

# 📊 Desafio de Clusterização RFV para E-commerce

## 🎯 Sobre o Projeto

Este projeto tem como objetivo principal segmentar clientes de um e-commerce utilizando técnicas de **clusterização**, com foco nas métricas **RFV** (Recência, Frequência e Valor Monetário).  
Através da análise do comportamento de compra, busco identificar padrões e características em comum entre os clientes, permitindo que a empresa personalize suas campanhas de marketing e otimize suas estratégias.

O desafio foi desenvolvido como parte de um programa de capacitação em Ciência de Dados, com foco em criar um modelo robusto e eficiente para análises de mercado.

---

## 📊 Contexto dos Dados

Os dados utilizados neste projeto são de transações de compras de uma loja de e-commerce, abrangendo operações em 38 países e territórios entre os anos de 2010 e 2011.  
A base de dados contém informações detalhadas sobre clientes, produtos e transações, totalizando mais de 4.000 clientes únicos e 540.000 transações.

**Fonte dos Dados:** [Kaggle - E-commerce Data](https://www.kaggle.com/datasets/carrie1/ecommerce-data)

---

## 📦 Estrutura dos Dados

| Coluna      | Descrição                             | Tipo      |
|-------------|---------------------------------------|-----------|
| InvoiceNo   | Identificação da transação            | Inteiro   |
| StockCode   | Código de estoque do produto          | String    |
| Description | Descrição do produto                  | String    |
| Quantity    | Quantidade de produtos por transação  | Inteiro   |
| InvoiceDate | Data da transação                     | Datetime  |
| UnitPrice   | Preço unitário do produto             | Float     |
| CustomerID  | Identificação do cliente              | Inteiro   |
| Country     | País de origem da transação           | String    |

---

## 🚀 Etapas do Desenvolvimento

### 1. Análise Exploratória dos Dados (EDA)
- Carregamento e descrição estatística inicial dos dados.
- Visualização das distribuições e avaliação da relevância das colunas.
- Identificação e tratamento de dados nulos, duplicados e outliers.
- Atenção especial ao formato das datas (MM/DD/YYYY HH:mm:ss) e à natureza dos IDs, que, embora numéricos, não devem ser tratados como grandezas numéricas.

### 2. Pré-processamento dos Dados
- Cálculo das métricas **RFV** (Recência, Frequência, Valor Monetário) para cada cliente.
- Normalização dos dados utilizando o **StandardScaler**, garantindo que todas as métricas tenham a mesma escala.
- Seleção das variáveis RFV para o modelo de clusterização.

### 3. Seleção e Implementação do Algoritmo de Clusterização
- Escolha do algoritmo **K-Means**, adequado para a segmentação de clientes com base nas métricas RFV.
- Determinação da quantidade ideal de clusters (k) utilizando o **Elbow Method**, uma técnica que identifica o ponto de inflexão da soma dos quadrados das distâncias (**WCSS**), indicando o número mais eficiente de agrupamentos.
- Implementação do **K-Means** com o valor otimizado de k.

### 4. Análise dos Clusters Obtidos
- Identificação dos padrões e características em comum entre os clientes de cada cluster.
- Utilização de gráficos e visualizações para auxiliar na interpretação dos resultados e compreensão dos diferentes perfis de clientes.

### 5. Interpretação e Recomendações
- Descrição detalhada do perfil de compra de cada cluster, fornecendo insights claros.
- Justificativa de como essa análise pode ser útil para a empresa em termos de **segmentação de clientes** e **personalização de campanhas de marketing**.
- Sugestões de **ações futuras** e estratégias direcionadas com base nos resultados dos clusters.

---

## ✨ Tecnologias Utilizadas

- **Python**: Linguagem de programação principal.
- **Pandas**: Manipulação e análise de dados.
- **NumPy**: Operações numéricas.
- **Matplotlib / Seaborn**: Visualização de dados.
- **Scikit-learn**: Pré-processamento e algoritmos de Machine Learning (ex: KMeans).

---

## 🚀 Como Executar o Projeto

### Clone o Repositório:

  - git clone https://github.com/SeuUsuario/NomeDoSeuRepositorio.git
  - cd NomeDoSeuRepositorio
  - Lembre-se de substituir SeuUsuario e NomeDoSeuRepositorio pelos seus dados reais.


### Abra o Notebook:
Você pode abrir o arquivo .ipynb diretamente no Google Colab (recomendado) ou localmente com Jupyter Notebook ou JupyterLab.

### Instale as Dependências:
Caso queira executar localmente:
pip install pandas numpy matplotlib seaborn scikit-learn
Execute as Células:
Siga o notebook célula por célula para replicar a análise e visualizar os resultados.

### 🤝 Contribuições
Sinta-se à vontade para explorar o código, sugerir melhorias ou abrir issues.
Contribuições são muito bem-vindas!

### 📧 Contato
LinkedIn: [Carlos Sotero](https://www.linkedin.com/in/carlos-sotero/)

Email: sotero.kka@gmail.com

📄 Licença
Este projeto está licenciado sob a Licença MIT. Consulte o arquivo LICENSE para mais detalhes.
