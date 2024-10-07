# Análise de Vendas

## Descrição do Projeto

Este projeto realiza a análise de dados consolidados de vendas utilizando a biblioteca `pandas` em Python. O objetivo é entender o desempenho das vendas em diferentes segmentos, produtos e países, permitindo a visualização das métricas de vendas, custo, lucro e margem de lucro.

## Estrutura dos Dados

Os dados utilizados para análise estão contidos em um arquivo Excel chamado `report-consolidado.xlsx`, que possui as seguintes colunas:

| Coluna                              | Descrição                                                            |
|-------------------------------------|----------------------------------------------------------------------|
| **Segmento**                        | Categoria da empresa (ex.: Governo, Grandes empresas, etc.)         |
| **País**                            | Localização geográfica das vendas                                    |
| **Produto**                         | Nome do produto vendido                                             |
| **Qtde de Unidades Vendidas**      | Quantidade total de unidades vendidas                                |
| **Preço Unitário**                 | Preço de venda por unidade                                          |
| **Valor Total**                     | Total gerado pelas vendas (Qtde de Unidades Vendidas * Preço Unitário) |
| **Desconto**                        | Total de descontos aplicados                                         |
| **Valor Total c/ Desconto**        | Total gerado após a aplicação de descontos                          |
| **Custo Total**                     | Custo total dos produtos vendidos                                    |
| **Lucro**                           | Diferença entre o Valor Total e o Custo Total                      |
| **Data**                            | Data da venda                                                       |
| **Mês**                             | Mês da venda                                                        |
| **Ano**                             | Ano da venda                                                        |

## Funcionalidades

- **Tratamento de Dados**: As colunas são padronizadas para facilitar a análise, removendo espaços e convertendo para letras minúsculas.
- **Análise por Segmento**: Os dados são agrupados por segmento, calculando o desconto total, custo total, lucro e margem de lucro.
- **Análise por Produto**: Os dados são agrupados por produto, com as mesmas métricas calculadas.
- **Análise por País**: Os dados são agrupados por país, apresentando também as métricas de desempenho.

## Resultados

Os resultados da análise são apresentados em DataFrames para cada agrupamento, onde as métricas calculadas são visualizadas de forma clara.

## Exemplo de Saída

```plaintext
segmento        desconto    custo_total    lucro    margem_lucro
Governo        3898805.83  41584282.5    10919978.17  280.09
Grandes empresas 1457305.62  20568882.0  -957187.63   -65.68
...

