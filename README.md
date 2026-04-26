# **MONITORAMENTO INTELIGENTE DE CONSUMO:**
REDUZINDO O DESPERDÍCIO NA INDÚSTRIA BRASILEIRA ATRAVÉS DE MODELAGEM PREDITIVA

---

## Objetivo

Analisar o comportamento do consumo energético ao longo do tempo e desenvolver um modelo preditivo para apoiar a compreensão da demanda.

---

## Dados

Base de dados com informações de consumo energético contendo:

- Data e hora (`din_instante`)
- Subsistema (`nom_subsistema`)
- Consumo (`val_cargaenergiamwmed`)

---

## Análise Exploratória

Foram realizadas análises para identificar:

- Tendência ao longo do tempo  
- Sazonalidade no consumo  
- Variabilidade dos dados  
- Dependência temporal (ACF e PACF)  

Também foi feita uma análise por subsistema, mostrando diferenças entre as regiões do país.

---

## Modelo Base

Foi aplicado um modelo ARIMA para previsão da série temporal.

- Divisão treino/teste  
- Geração de previsões  
- Avaliação com MAE e RMSE  

O modelo conseguiu capturar o comportamento geral da série, com limitações em variações mais complexas.

---

## Integrantes

- Felipe Graciano de Moura Ramos  
- João Pedro Rocha Abbade  
- Marcos Davi Duarte Abibe  
- Thais Jorge Azevedo  
