# NAVI — Copiloto Inteligente de Viagem

Projeto desenvolvido para a disciplina de Inteligência Artificial e Aprendizagem de Máquina.

A NAVI é um copiloto inteligente de viagem que integra reconhecimento de voz, análise de emoções, visão computacional, localização e contexto da viagem para gerar recomendações por meio de Machine Learning.

## Objetivo

Criar um sistema multimodal capaz de auxiliar o usuário durante uma viagem, analisando diferentes tipos de entrada e gerando recomendações de acordo com o contexto.

## Fluxo do sistema

Comando de voz → Emoção → Imagem → Localização → Random Forest → Recomendação → Registro

## Funcionalidades

- Reconhecimento de comandos por voz
- Palavra de ativação "NAVI"
- Classificação de emoção pela voz
- Reconhecimento de contexto por imagem
- Registro da localização
- Análise do contexto da viagem
- Geração de recomendações com Random Forest
- Diário de bordo automático
- Resumo da viagem

## Comandos disponíveis

- "Navi, registrar parada"
- "Navi, preciso abastecer"
- "Navi, registrar paisagem"
- "Navi, como está a viagem?"

## Emoções analisadas

- Animado
- Tenso
- Neutro
- Cansado

## Classes de imagem

- Estrada / rodovia
- Posto de combustível
- Restaurante / alimentação
- Natureza / ponto turístico

## Variáveis utilizadas pelo Random Forest

- Tempo de viagem
- Distância percorrida
- Tempo desde a última parada
- Emoção vocal
- Contexto da imagem
- Horário

## Possíveis recomendações

- CONTINUAR
- DESCANSAR
- ABASTECER
- ALIMENTAR-SE
- REGISTRAR PONTO TURÍSTICO

## Tecnologias utilizadas

- Python
- Flask
- HTML
- CSS
- JavaScript
- Scikit-learn
- NumPy
- Librosa
- SpeechRecognition
- Pillow
- OpenCV
- Random Forest
- SVM
- Extra Trees

## Machine Learning

O projeto utiliza modelos treinados com datasets próprios para:

- classificação de emoções pela voz;
- classificação de imagens;
- geração de recomendações com Random Forest.

As decisões não são hardcoded. Os modelos realizam previsões com base nas entradas recebidas pelo sistema.

## Estrutura do projeto

```text
NAVI/
├── navi_web.py
├── dataset_emocoes/
├── dataset_imagens/
├── modelos/
├── fotos_navi/
├── diario_bordo_navi.csv
└── demais arquivos do projeto
