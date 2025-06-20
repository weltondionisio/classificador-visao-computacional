# Classificador de Imagens: Gatos vs Cachorros 🐱🐶

Este projeto utiliza redes neurais convolucionais (CNN) para classificar imagens de gatos e cachorros, comparando uma arquitetura criada do zero com uma abordagem de Transfer Learning usando ResNet18 pré-treinada.

---

## Sobre o Projeto

O objetivo é comparar o desempenho de uma CNN simples, desenvolvida manualmente, com um modelo de Transfer Learning (ResNet18) para o problema de classificação binária de imagens (gatos vs cachorros).

- **CNN Simples:** Arquitetura customizada, treinada do zero, com ajuste de hiperparâmetros via GridSearchCV.
- **Transfer Learning:** Utiliza ResNet18 pré-treinada no ImageNet, ajustando apenas a última camada para o problema binário.

## Como Executar

1. **Clone o repositório:**
   git clone https://github.com/weltondionisio/classificador-visao-computacional.git
   cd classificador-visao-computacional
   
2. Instale as dependências:
   pip install -r requirements.txt

3. Execute o notebook: Abra o arquivo CNN_Cats_vs_Dogs.ipynb no Jupyter Notebook ou VS Code e siga as células.

4. Baixe o dataset automaticamente: O notebook faz o download do dataset via kagglehub.

5. Estrutura do Projeto
classificador-visao-computacional/
│
├── CNN_Cats_vs_Dogs.ipynb   # Notebook principal do projeto
├── requirements.txt         # (Opcional) Dependências do projeto
└── README.md                # Este arquivo

## Resultados
CNN Simples:
- Acurácia no teste: ~50%
- Loss final: (veja no notebook)
Transfer Learning (ResNet18):
- Acurácia no teste: ~98%
- Loss final: muito menor que a CNN simples

O Transfer Learning se destacou, mostrando grande capacidade de generalização mesmo com poucas épocas de treino, graças ao conhecimento prévio do ImageNet.

## Autor
Projeto desenvolvido por [Welton Dionisio](https://github.com/weltondionisio).
