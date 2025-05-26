# Representações Latentes com Autoencoders

Os **Autoencoders** são redes neurais artificiais utilizadas para **aprender representações compactas e eficientes dos dados** (codificação), com o objetivo de reconstruir a entrada original o mais fielmente possível.

Eles são amplamente usados para **compressão, remoção de ruído, pré-treinamento e geração de dados sintéticos**, funcionando como uma espécie de filtro de informação.

### Por que Autoencoders são úteis?

- Aprendem **representações latentes** dos dados de forma não supervisionada
- Permitem **redução de dimensionalidade** preservando informações relevantes
- São base para modelos geradores como **Variational Autoencoders (VAEs)**
- Aplicáveis em **reconstrução de imagens, remoção de ruído e detecção de anomalias**

### Funcionamento Intuitivo

Pense em um **autoencoder como um tradutor eficiente**: ele pega uma imagem de entrada, "traduza" para uma versão reduzida com as informações mais importantes (camada latente) e depois reconstrói a imagem original a partir dessa versão compacta.

---

## 📂 Estrutura dos Notebooks

### 1. `AE1_CIPAR10_Autoencoder_Orlando.ipynb`
**📌 Tarefa:** Reconstrução de imagens do dataset CIFAR-10  
**📚 Dataset:** [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)  
**🔍 Destaques:**
- Codificação de imagens RGB
- Comparação visual entre imagens originais e reconstruídas
- Visualização do espaço latente

### 2. `AE2_simples_digitos_Orlando.ipynb`
**📌 Tarefa:** Reconstrução de dígitos manuscritos com arquitetura simples  
**📚 Dataset:** [MNIST](http://yann.lecun.com/exdb/mnist/)  
**🔍 Destaques:**
- Arquitetura leve com codificador e decodificador simétricos
- Visualização de reconstruções dígito a dígito
- Avaliação por erro de reconstrução

### 3. `AE3_Deep_Autoencoder_Orlando.ipynb`
**📌 Tarefa:** Compressão profunda de imagens com autoencoder empilhado  
**📚 Dataset:** MNIST ou CIFAR-10 (verificado automaticamente no notebook)  
**🔍 Destaques:**
- Múltiplas camadas densas no encoder e decoder
- Codificação em dimensões muito reduzidas
- Análise da performance na reconstrução

---

## 📈 Métricas e Avaliação

Os autoencoders são avaliados por:

- **Erro de reconstrução** (ex: MSE)
- **Capacidade de compressão** (dimensão latente vs. original)
- **Visualização das imagens reconstruídas**
- **Percepção visual da fidelidade na reconstrução**

---

## ⚙️ Técnicas Utilizadas

- Arquiteturas simétricas Encoder-Decoder
- Função de ativação ReLU e Sigmoid
- Otimizadores como Adam
- Visualizações com Matplotlib
"""
