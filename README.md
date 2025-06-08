# Fundamentos Matemáticos dos Algoritmos de Machine Learning

Este repositório tem como objetivo apresentar os fundamentos matemáticos por trás dos principais algoritmos de Machine Learning. A proposta é oferecer uma abordagem didática e aprofundada, conectando teoria e prática por meio de conteúdos matemáticos e implementações em Python.

## 🔍 Objetivos

- Explorar os conceitos fundamentais de Álgebra Linear, Cálculo, Estatística e Otimização aplicados ao aprendizado de máquina.
- Apresentar a dedução matemática e a lógica por trás de algoritmos clássicos.
- Disponibilizar notebooks interativos com explicações passo a passo e códigos funcionais.
- Servir como base para estudos autodidatas, cursos, workshops ou disciplinas na área de IA.

---

## ✅ Algoritmos abordados (em desenvolvimento)

- [x] Regressão Linear
- [ ] Regressão Logística
- [ ] K-Means
- [ ] Support Vector Machines (SVM)
- [ ] Redes Neurais
- [ ] Árvores de Decisão
- [ ] PCA (Análise de Componentes Principais)

---

## 📘 1. Regressão Linear

### 💡 Intuição

A regressão linear é um modelo supervisionado utilizado para prever uma variável contínua a partir de uma ou mais variáveis independentes. A ideia central é ajustar uma reta (ou hiperplano) que melhor representa a tendência dos dados.

### 📐 Formulação Matemática

O modelo é dado por:

\[
\hat{y} = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \cdots + \beta_n x_n
\]

ou, em notação vetorial:

\[
\hat{y} = \mathbf{X}\boldsymbol{\beta}
\]

Onde:
- \(\mathbf{X}\) é a matriz de entrada (com uma coluna de 1s para o termo de bias),
- \(\boldsymbol{\beta}\) é o vetor de coeficientes a serem aprendidos.

### 🎯 Função de Custo

A função de custo usada é o **Erro Quadrático Médio (MSE)**:

\[
J(\boldsymbol{\beta}) = \frac{1}{2m} \sum_{i=1}^{m} (\hat{y}^{(i)} - y^{(i)})^2
\]

O objetivo do algoritmo é minimizar essa função.

### ⚙️ Solução Analítica

A minimização da função de custo pode ser feita de forma fechada por:

\[
\boldsymbol{\beta} = (\mathbf{X}^T \mathbf{X})^{-1} \mathbf{X}^T \mathbf{y}
\]

### 💻 Implementação em Python

Você pode conferir a implementação detalhada em [notebooks/regressao_linear.ipynb](notebooks/regressao_linear.ipynb), onde apresentamos:
- Geração de dados sintéticos
- Ajuste manual dos parâmetros
- Solução com equação normal
- Comparação com `scikit-learn`

---

## 📁 Estrutura do Repositório

