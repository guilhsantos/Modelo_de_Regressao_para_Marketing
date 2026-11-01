🇧🇷 **Português** · [🇺🇸 English](README.en.md)

# Regressão para investimento em marketing

Modelo que estima as vendas a partir do investimento em YouTube, Facebook e jornal, para apoiar a decisão de onde colocar a verba.

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guilhsantos/Modelo_de_Regressao_para_Marketing/blob/main/Modelo_de_Regress%C3%A3o_para_Marketing.ipynb)

## Problema

A empresa investe todo mês em três canais de mídia, mas não sabe quanto cada um contribui para as vendas nem quanto esperar de retorno de um novo plano de investimento.

## Solução

Regressão linear treinada com o histórico de investimento e vendas (`MKT.csv`), que recebe um plano de mídia e devolve a venda prevista.

## Resultado

No conjunto de teste (20% da base):

| Métrica | Valor |
|---|---|
| **R²** | **0,87**: o modelo explica 87% da variação das vendas |
| RMSE | 2,36 (na unidade de vendas da base) |
| MSE | 5,58 |

O notebook termina com um simulador: você informa o investimento em cada canal e recebe a venda prevista.

## Como fiz

1. **Análise descritiva:** estrutura, nulos e estatísticas de cada canal.
2. **Análise exploratória:** pairplot e matriz de correlação entre investimento e vendas.
3. **Modelagem:** regressão linear (scikit-learn) com divisão 80/20 entre treino e teste.
4. **Avaliação:** MSE, RMSE, R² e gráfico de real × previsto.
5. **Predição:** teste com valores novos de investimento.

## Próximos passos

- Ler os coeficientes para dizer quanto cada real a mais em cada canal rende em vendas.
- Testar interação entre canais e retornos decrescentes, porque investir o dobro raramente vende o dobro.

## Stack

Python · pandas · NumPy · scikit-learn · Seaborn · Matplotlib · Google Colab

---

Feito por [Guilherme Santos](https://portifolio-guilherme-santos.vercel.app) · [LinkedIn](https://www.linkedin.com/in/guilherme-santos-dataeng)
