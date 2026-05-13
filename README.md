# 🚗 Previsão de Preço de Veículos Usados

Modelo de regressão linear múltipla para prever o preço de veículos usados, com pipeline completo de limpeza, EDA e avaliação em Python.

## Sobre o projeto

Uma plataforma de compra e venda de veículos usados precisa estimar automaticamente o preço de um anúncio no momento do cadastro. Este projeto constrói um modelo preditivo treinado com dados históricos de transações, eliminando a necessidade de avaliação manual.

## Estrutura

```
├── Regressao_Veiculos.ipynb   # notebook principal
└── BD_veiculos_2.csv          # dataset com ~1000 transações
```

## Pipeline

1. **Carregamento e inspeção** — shape, nulos, tipos e estatísticas descritivas
2. **Limpeza de dados** — erros de digitação, valores nulos, fora do domínio e inconsistências lógicas
3. **EDA** — distribuição do preço, correlações, boxplots por tipo/marca/câmbio e scatter plots
4. **Pré-processamento** — One-Hot Encoding, split 80/20 e StandardScaler
5. **Treinamento** — Regressão Linear Múltipla (OLS) com análise de coeficientes
6. **Avaliação** — MAE, RMSE, R², R² ajustado, análise de resíduos e validação cruzada 10-fold
7. **Desafio extra** — transformação log do target, engenharia de features e comparação Ridge/Lasso

## Resultados

| Métrica | Valor |
|---|---|
| MAE | calculado ao executar |
| RMSE | calculado ao executar |
| R² | calculado ao executar |
| CV 10-fold RMSE | calculado ao executar |

> Os valores dependem do dataset e são exibidos ao rodar o notebook.

## Tecnologias

- Python 3.10+
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## Como executar

```bash
# clone o repositório
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo

# instale as dependências
pip install pandas numpy scikit-learn matplotlib seaborn

# abra o notebook
jupyter notebook Regressao_Veiculos.ipynb
```

Certifique-se de que o arquivo `BD_veiculos_2.csv` está na mesma pasta do notebook antes de executar.
