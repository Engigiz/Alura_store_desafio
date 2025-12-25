# Análise de Vendas Multiloja

Este projeto realiza uma análise exploratória de dados de vendas de quatro lojas distintas, focando-se em métricas de faturação, desempenho por categoria e custos logísticos.

## 📋 Descrição do Projeto

O objetivo deste notebook é consolidar dados de diferentes fontes e extrair *insights* sobre o comportamento de vendas e custos de frete entre diferentes unidades de negócio. Os dados são carregados a partir de repositórios externos (GitHub) e processados individualmente para comparação.

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **Pandas**: Manipulação e tratamento de dados.
* **Matplotlib**: Visualização de dados (gráficos).

## 📊 Análises Realizadas

O ficheiro `analise.ipynb` executa os seguintes passos:

1.  **Importação e Inspeção**: Carregamento de 4 datasets (`loja_1`, `loja_2`, `loja_3`, `loja_4`) e verificação da integridade dos dados através dos métodos `.head()` e `.info()`.
2.  **Cálculo de Faturação**: Soma do valor total de vendas (coluna `Preço`) para cada uma das quatro lojas.
3.  **Vendas por Categoria**: Identificação dos segmentos mais vendidos (como móveis, eletrónicos e brinquedos) através do agrupamento por `Categoria do Produto`.
4.  **Análise de Frete**: Cálculo da média de custos de envio por loja, com a geração de um gráfico de barras horizontais para comparação visual.

## 📂 Estrutura dos Dados

Os ficheiros analisados contêm as seguintes colunas principais:
* `Produto`: Nome do item vendido.
* `Categoria do Produto`: Segmento do produto.
* `Preço`: Valor da venda.
* `Frete`: Custo de transporte.
* `Vendedor`: Nome do responsável pela venda.
* `Local da compra`: Estado (UF) onde a venda foi realizada.

## 🚀 Como Executar

1.  Instale as dependências:
    ```bash
    pip install pandas matplotlib
    ```
2.  Abra o notebook `analise.ipynb` em um ambiente Jupyter ou VS Code.
3.  Execute as células sequencialmente para visualizar as métricas e gráficos.