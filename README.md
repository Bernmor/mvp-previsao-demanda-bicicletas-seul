# MVP - Previsão de Demanda de Bicicletas Compartilhadas em Seul

Este repositório contém um MVP de Machine Learning desenvolvido para prever a demanda horária de bicicletas compartilhadas na cidade de Seul, utilizando o dataset público **Seoul Bike Sharing Demand**.

O projeto foi desenvolvido em Python, no formato de notebook, e apresenta o fluxo essencial de um projeto de aprendizado de máquina: definição do problema, apresentação dos dados, análise exploratória, preparação das variáveis, divisão temporal, treinamento de modelos, otimização de hiperparâmetros, avaliação em dados não vistos e discussão crítica dos resultados.

## Objetivo

Construir e avaliar modelos de regressão capazes de estimar a quantidade de bicicletas alugadas por hora, considerando variáveis de calendário, clima, estação do ano, feriados e funcionamento do serviço.

## Conteúdo do Projeto

- Análise exploratória dos dados.
- Preparação e transformação de variáveis.
- Engenharia de atributos temporais e climáticos.
- Divisão cronológica em treino, validação e teste.
- Construção de modelos baseline e modelos candidatos.
- Comparação entre Ridge, PCA + Ridge, Random Forest e HistGradientBoosting.
- Otimização de hiperparâmetros com validação temporal.
- Avaliação final com MAE, RMSE e R².
- Análise de erros e interpretação das variáveis mais relevantes.
- Discussão de limitações e próximos passos.

## Dataset

O dataset utilizado é o **Seoul Bike Sharing Demand**, disponibilizado originalmente pela UCI Machine Learning Repository.

Para garantir reprodutibilidade na entrega, uma cópia do arquivo CSV foi incluída em `data/SeoulBikeData.csv`. O notebook carrega os dados diretamente pela URL pública raw deste repositório:

`https://raw.githubusercontent.com/Bernmor/mvp-previsao-demanda-bicicletas-seul/main/data/SeoulBikeData.csv`

## Arquivo Principal

- `seoul_bike_demand_mvp.ipynb`: notebook principal do MVP, contendo código, visualizações, métricas e explicações textuais.

## Como Executar

1. Abra o notebook `seoul_bike_demand_mvp.ipynb` no Google Colab.
2. Confirme que a URL do dataset no notebook aponta para a versão raw deste repositório.
3. Execute todas as células em ordem, usando `Runtime > Run all`.

O notebook foi estruturado para ser executado sem upload manual de arquivos, sem credenciais privadas e sem configuração local adicional.

## Resultado Esperado

Ao final da execução, o notebook apresenta a comparação entre modelos, a escolha da melhor solução com base no MAE de validação, a avaliação final no conjunto de teste e uma discussão crítica sobre limitações, riscos de generalização e oportunidades de melhoria.
