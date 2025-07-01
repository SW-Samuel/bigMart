# 📊 Big Mart Sales Prediction

Este repositório contém uma análise preditiva completa aplicada ao conjunto de dados do [Big Mart Sales](https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets). O objetivo é prever as vendas de cada produto com base em variáveis relacionadas ao item e à loja.

![bigmart-banner](https://upload.wikimedia.org/wikipedia/commons/thumb/3/30/Bigmart_Supermarket.jpg/640px-Bigmart_Supermarket.jpg)

---

## 🔍 Sobre o Projeto

A previsão de vendas é uma tarefa fundamental no varejo. O desafio proposto neste projeto é construir um modelo que possa prever `Item_Outlet_Sales` com base em atributos como tipo de item, visibilidade, tipo de loja, localização, etc.

Este projeto:

- Realiza uma **análise exploratória dos dados (EDA)**
- Trata valores ausentes e inconsistências
- Cria um modelo preditivo com **XGBoost** e **Random Forest**
- Avalia os modelos com métricas como **RMSE** e **R²**
- Compara o desempenho dos modelos com um **baseline simples**

---

## 📊 Principais Etapas da Análise

### 🔹 1. Análise Exploratória (EDA)
- Visualizações de distribuição de vendas
- Agrupamentos por tipo de item e loja
- Testes estatísticos (ANOVA e t-test)

### 🔹 2. Pré-processamento
- Tratamento de valores ausentes (`Item_Visibility`, `Outlet_Size`)
- Codificação de variáveis categóricas com `get_dummies`
- Criação de variáveis úteis para o modelo

### 🔹 3. Modelagem
- **Baseline** com média de vendas
- **Random Forest Regressor**
- **XGBoost Regressor (API nativa)** com early stopping
- Avaliação com RMSE, MAE, R²

### 🔹 4. Comparação de Modelos

| Modelo            | R²       | RMSE       |
|------------------|----------|------------|
| Baseline         | -0.0039  | 2,513,784.0 |
| Random Forest    | 0.6250   | 1,021.95    |
| XGBoost (nativo) | **0.6250** | **969.00**  |

---

## ✅ Conclusão

O modelo com melhor desempenho foi o **XGBoost** com ajuste de hiperparâmetros e early stopping. Ele apresentou o menor erro quadrático médio (RMSE) e bom poder explicativo (R²), tornando-se o mais indicado para prever vendas no contexto do problema.

---

## 📌 Fonte dos Dados

Dataset original disponível em:  
👉 [Kaggle - Big Mart Sales Dataset](https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets)

---

## 📧 Contato

Projeto desenvolvido por **SW Samuel**  
GitHub: [@SW-Samuel](https://github.com/SW-Samuel)
