# 



# Monitoramento Inteligente de Consumo Energético

Projeto desenvolvido na disciplina **Projeto Aplicado IV** com o objetivo de analisar e prever o consumo de energia elétrica no Brasil utilizando técnicas de séries temporais.

---

## Objetivo

Este projeto tem como objetivo identificar padrões de consumo energético e desenvolver um modelo preditivo capaz de antecipar o comportamento da demanda, contribuindo para a **redução de desperdícios energéticos** e apoio à tomada de decisão.

---

## Base de Dados

Os dados utilizados foram obtidos de fontes oficiais do setor elétrico brasileiro:

- ONS (Operador Nacional do Sistema Elétrico)
- CCEE (Câmara de Comercialização de Energia Elétrica)

A base contém:

- Data e hora (`din_instante`)
- Subsistema (`nom_subsistema`)
- Consumo de energia (`val_cargaenergiamwmed`)

---

## Pipeline do Projeto

O projeto foi estruturado seguindo as etapas abaixo:

1. Coleta de Dados  
2. Pré-processamento  
3. Análise Exploratória (EDA)  
4. Análise de Séries Temporais (ACF, PACF, decomposição)  
5. Modelagem Preditiva (ARIMA)  
6. Avaliação dos Modelos  
7. Geração de Insights  

---

## Análise Exploratória (EDA)

Durante a análise exploratória, foram identificados:

- Tendência ao longo do ano  
- Forte sazonalidade diária  
- Alta variabilidade nos dados  
- Dependência temporal (ACF/PACF)  

A decomposição da série evidenciou:

- Tendência não linear  
- Componente sazonal forte  
- Resíduo aleatório  

---

## Análise por Subsistema

A segmentação por região revelou diferenças relevantes:

- Sudeste/Centro-Oeste → maior consumo  
- Sul → comportamento semelhante, menor escala  
- Nordeste → mais estável  
- Norte → menor consumo  

Essa análise destaca a importância de considerar **características regionais** na modelagem.

---

## Modelo Base

Foi implementado um modelo **ARIMA (2,1,2)** para previsão da série temporal.

### Metodologia:

- Divisão treino/teste (80/20)  
- Treinamento do modelo  
- Geração de previsões  

### Resultados:

- MAE: ~1285  
- RMSE: ~1481  

O modelo demonstrou capacidade de capturar o comportamento geral da série, embora apresente limitações na modelagem de padrões sazonais mais complexos.

---

## Insights

- O consumo energético apresenta forte padrão cíclico  
- Há diferenças relevantes entre regiões  
- Modelos preditivos podem apoiar estratégias de eficiência energética  
- Possível aplicação em monitoramento industrial e redução de desperdícios  

---

## Próximos Passos

- Implementação de modelo **SARIMA**  
- Uso de variáveis exógenas (ex: clima)  
- Teste com modelos de Machine Learning  
- Otimização de parâmetros  

---

## Tecnologias Utilizadas

- Python  
- Pandas  
- Matplotlib  
- Statsmodels  
- Scikit-learn  

---

## Integrantes

- Felipe Graciano de Moura Ramos  
- João Pedro Rocha Abbade  
- Marcos Davi Duarte Abibe  
- Thais Jorge Azevedo  
