# 🧠 VAE com Fashion MNIST – Geração e Reconstrução de Imagens com TensorFlow

Este projeto implementa um **Autoencoder Variacional (VAE)** usando a base de dados **Fashion MNIST**, com o objetivo de gerar e reconstruir imagens de artigos de moda de forma realista. Ele utiliza camadas convolucionais e a técnica de reparametrização para criar um modelo probabilístico poderoso, aplicando princípios de aprendizado não supervisionado.

---

## 🧩 Visão Geral

- 🎯 **Objetivo:** Demonstrar o uso de um VAE com camadas convolucionais para gerar imagens sintéticas e realizar reconstrução de imagens reais.
- 🧪 **Base de Dados:** [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) — 70.000 imagens em escala de cinza de 28x28 pixels representando roupas e acessórios.
- ⚙️ **Técnicas Utilizadas:**
  - Convolutional Variational Autoencoder (CVAE)
  - Reparametrização (z = μ + σ * ε)
  - Loss personalizada combinando **Binary Crossentropy** + **KL Divergence**
  - Visualização de aprendizado e amostragem de espaço latente
  - Medição de tempo de treinamento por batch

---

## 🛠️ Ferramentas e Tecnologias

| Tecnologia | Função |
|------------|--------|
| Python 3.x | Linguagem principal |
| TensorFlow / Keras | Framework de Deep Learning |
| NumPy | Manipulação de arrays |
| Matplotlib | Visualização de dados |
| Fashion MNIST | Dataset de benchmark |

---

## 📚 Conceitos Importantes

### 🔍 O que é um VAE?

Um **Variational Autoencoder (VAE)** é uma rede neural generativa que aprende uma representação **probabilística** dos dados. Ele codifica os dados de entrada em uma distribuição latente, permitindo a geração de novas amostras similares às originais.

### ⚖️ Função de Perda

A perda total do modelo combina:

- **Reconstruction Loss:** Mede quão parecida a imagem reconstruída é com a original (via Binary Crossentropy).
- **KL Divergence:** Penaliza desvios da distribuição latente aprendida em relação a uma distribuição normal padrão.

---

## 🖼️ Exemplos de Resultados

### 🎲 Amostras Sintéticas

#### 🔷 Amostra Sintética Única
![img_sintetica_unica](https://github.com/user-attachments/assets/60fabe6e-c4cc-49fb-b454-70d47e18183e)

#### 🔶 256 Amostras SIntéticas Aleatórias
![img_sinteticas](https://github.com/user-attachments/assets/b519dbaf-552e-46e1-90d8-5c9976d142ff)

---

## 💡 Aplicações Reais

- **Compressão de imagens**
- **Remoção de ruído**
- **Geração de conteúdo visual**
- **Análise de anomalias em imagens**
- **Base para modelos de transferência de estilo**

---

## 📈 Métricas de Desempenho

Durante o treinamento, foram monitoradas:

- `total_loss` (perda total)
- `ce_loss` (reconstruction loss)
- `kl_loss` (KL divergence loss)
- `training_time` (tempo por batch)

Essas métricas ajudam a compreender o comportamento do modelo ao longo das épocas e verificar se ele está aprendendo uma distribuição significativa.
---

## 📧 Contato

- 📌 **Autor**: Hian Stafford
- 📩 **Email**: hian.correa@gmail.com
```text
  /\_/\  
 ( -.- ) 
  > ^ < 
```
