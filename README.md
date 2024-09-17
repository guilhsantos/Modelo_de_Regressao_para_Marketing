# Análise e Modelagem de Dados de Marketing
## Descrição do Projeto
A empresa realiza investimentos mensais em publicidade online (YouTube, Facebook e jornais) e registra os gastos e retornos de vendas. O objetivo deste projeto é analisar a relação entre esses investimentos e as vendas para identificar quais variáveis impactam mais as vendas e criar um modelo de regressão linear para prever o retorno das vendas baseado em novos investimentos.

## Dataset Utilizado
O dataset utilizado foi o MKT.csv, que contém informações sobre investimentos em marketing e vendas. As colunas principais são:

- youtube: Investimento em publicidade no YouTube
- facebook: Investimento em publicidade no Facebook
- newspaper: Investimento em publicidade em jornais
- sales: Vendas resultantes dos investimentos em marketing
# Passos Realizados
## Passo 1: Análise Descritiva
No primeiro passo, conectei ao Google Drive para carregar o dataset MKT.csv. Em seguida, importei as bibliotecas necessárias, como Pandas, NumPy, Seaborn, Matplotlib e SKLEARN, para manipulação de dados e modelagem. O dataset foi carregado e suas primeiras linhas foram visualizadas para entender a estrutura dos dados. Realizei a análise das informações gerais do dataset, incluindo a identificação de valores nulos. Além disso, foram geradas estatísticas descritivas para entender a distribuição dos investimentos e das vendas.
## Passo 2: Análise Exploratória
No segundo passo, realizei a análise exploratória dos dados. Gere estatísticas descritivas e um pairplot para examinar a relação entre os investimentos e as vendas. Também criei uma matriz de correlação para identificar as relações entre as variáveis e destacar os relacionamentos significativos.
## Passo 3: Modelagem
No terceiro passo, implementei um modelo de regressão linear utilizando a biblioteca SKLEARN. O dataset foi dividido em 80% para treino e 20% para teste. Avaliei o modelo usando métricas como MSE (Mean Squared Error), RMSE (Root Mean Squared Error) e R² (Coeficiente de Determinação) para verificar a precisão e o ajuste do modelo.
## Passo 4: Predição
No quarto passo, utilizei o modelo treinado para fazer predições com novos dados e comparei esses valores com os reais para avaliar o desempenho do modelo. Também realizei um teste de predição com novos valores de investimento para verificar a capacidade do modelo em estimar o retorno das vendas.
## Resultados
- MSE Linear: 5.57
- RMSE Linear: 2.36
- R² Linear: 0.87
  
O gráfico de dispersão dos valores reais x valores preditos mostra a qualidade do ajuste do modelo.

## Conclusão
O modelo de regressão linear foi capaz de prever as vendas com base nos investimentos em marketing, e as métricas de avaliação indicam a eficácia do modelo.
