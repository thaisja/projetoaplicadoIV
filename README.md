# Monitoramento Inteligente de Consumo

Projeto desenvolvido na disciplina de Projeto Aplicado IV com foco na análise e previsão do consumo energético brasileiro utilizando técnicas de séries temporais.

## Objetivo

Desenvolver um modelo preditivo capaz de analisar padrões de consumo energético no Brasil, auxiliando no monitoramento inteligente e na redução de desperdícios.

---

## Base de Dados

Base pública de carga energética do Brasil disponibilizada por:

* ONS (Operador Nacional do Sistema)
* CCEE (Câmara de Comercialização de Energia Elétrica)

### Variáveis utilizadas

* Data e hora
* Subsistema
* Consumo energético (MW)

### Período analisado

* Ano de 2025
* Granularidade horária

---

## Etapas do Projeto

### 1. Pré-processamento

* Conversão de datas
* Organização temporal
* Limpeza e preparação dos dados

### 2. Análise Exploratória

* Consumo médio diário
* Identificação de sazonalidade
* Análise por subsistema
* Estatísticas descritivas

### 3. Decomposição da Série Temporal

* Tendência
* Sazonalidade
* Resíduos

### 4. Modelagem Preditiva

Modelos implementados:

* ARIMA
* SARIMA

### 5. Avaliação dos Modelos

Métricas utilizadas:

* MAE
* RMSE

Resultados obtidos:

| Modelo | MAE     | RMSE    |
| ------ | ------- | ------- |
| ARIMA  | 1285.40 | 1481.55 |
| SARIMA | 3654.56 | 4151.70 |

O modelo ARIMA apresentou melhor desempenho para a série analisada.

---

## Tecnologias Utilizadas

* Python
* Pandas
* Matplotlib
* Statsmodels
* Jupyter Notebook

---

## Estrutura do Repositório

```bash
📁 notebooks
📁 dados
📁 apresentacao
📄 README.md
```
---

## Apresetação
https://youtu.be/jCawjIumK1M

---

## Integrantes

* Felipe Graciano de Moura Ramos
* João Pedro Rocha Abbade
* Marcos Davi Duarte Abibe
* Thais Jorge Azevedo

---

## Trabalhos Futuros

* Inclusão de variáveis meteorológicas
* Teste com modelos de machine learning
* Dashboard em tempo real
* Expansão da base histórica

