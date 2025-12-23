# Projetos de Deep Learning: Imagem, Texto e Modelos Generativos
> Trabalho realizado para a disciplina: Deep Learning, no curso de Inteligência Artifical Aplicada da UFPR

Este repositório contém uma coleção de projetos práticos de Deep Learning desenvolvidos em Python utilizando a biblioteca **TensorFlow/Keras**. Os projetos abrangem desde a classificação clássica de imagens e processamento de linguagem natural (NLP) até modelos avançados de arquitetura Transformer e Redes Adversárias Generativas (GANs).

## 🚀 Projetos Incluídos

### 1. Classificação de Imagens com CNN

* **Notebook:** `1_Classificação_de_Imagens_(CNN).ipynb`
* **Objetivo:** Classificar imagens coloridas em 10 categorias distintas.
* **Dataset:** [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) (60.000 imagens de 32x32 pixels).
* **Arquitetura:** Rede Neural Convolucional (CNN) com camadas de convolução, Dropout para evitar overfitting e camadas densas.
* **Tecnologias:** TensorFlow, NumPy, Matplotlib, Scikit-learn (matriz de confusão).

### 2. Detector de SPAM com RNN (LSTM)

* **Notebook:** `2_Detector_de_SPAM_(RNN).ipynb`
* **Objetivo:** Identificar se mensagens de texto são legítimas (*ham*) ou SPAM.
* **Dataset:** Base de dados de SMS com rótulos binários.
* **Arquitetura:** Rede Neural Recorrente (RNN) utilizando uma camada de **Embedding** seguida por uma célula **LSTM** (*Long Short-Term Memory*) para capturar o contexto sequencial das palavras.
* **Tecnologias:** TensorFlow, Pandas (manipulação de dados), Scikit-learn.

### 3. Gerador de Dígitos "Fake" com GAN

* **Notebook:** `3_Gerador_de_Dígitos_Fake_(GAN).ipynb`
* **Objetivo:** Treinar uma rede para criar imagens inéditas de dígitos escritos à mão que pareçam reais.
* **Dataset:** [MNIST](http://yann.lecun.com/exdb/mnist/).
* **Arquitetura:** **DCGAN** (Deep Convolutional Generative Adversarial Network). Consiste em dois modelos competindo:
* **Gerador:** Cria imagens a partir de ruído aleatório.
* **Discriminador:** Tenta distinguir entre imagens reais do dataset e imagens falsas criadas pelo gerador.
* **Tecnologias:** TensorFlow, ImageIO (criação de GIFs do treinamento), PIL.

### 4. Tradutor de Textos com Transformer

* **Notebook:** `4_Tradutor_de_Textos_(Transformer).ipynb`
* **Objetivo:** Tradução automática de sentenças do Português para o Inglês.
* **Dataset:** Dataset da TED Talks fornecido pelo TensorFlow Datasets.
* **Arquitetura:** Arquitetura **Transformer** completa, baseada no artigo *"Attention is All You Need"*. Inclui:
* Atenção de múltiplas cabeças (Multi-head Attention).
* Codificação Posicional (Positional Encoding).
* Máscaras de preenchimento e antecipação (Padding and Look-ahead masks).


* **Tecnologias:** TensorFlow Text, TensorFlow Datasets, NumPy.

## 🛠️ Pré-requisitos

Para executar os notebooks, você precisará das seguintes bibliotecas principais instaladas:

```bash
pip install tensorflow tensorflow-datasets tensorflow-text numpy matplotlib pandas scikit-learn imageio

```

## 📈 Como Executar

1. Certifique-se de ter um ambiente com suporte a GPU (altamente recomendado para a GAN e o Transformer, como o Google Colab).
2. Abra o notebook desejado no ambiente Jupyter ou Colab.
3. Execute as células em ordem. Os notebooks estão configurados para baixar automaticamente os datasets necessários através das APIs do TensorFlow.

---
