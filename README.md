# VisusAI - Deep Learning Training Pipeline 🧠

Repositório dedicado à engenharia e treinamento do modelo de Visão Computacional para detecção de Retinopatia Diabética.

## 🔬 O Modelo
Utilizei a **EfficientNet-B4** (PyTorch Image Models - timm) com Transfer Learning.

## ⚙️ Pipeline de Treinamento
Este projeto resolve desafios comuns de datasets médicos:

1.  **Pré-processamento (CLAHE):** Aplicação de contraste adaptativo para realçar microaneurismas.
2.  **Resolução:** Input de 512x512px (acima do padrão 224px).
3.  **Balanceamento:** Uso de `WeightedRandomSampler` para corrigir o desbalanceamento severo entre classes "Normal" e "Proliferativa".

## 📂 Estrutura
* `notebooks/`: Jupyter Notebooks com a análise exploratória e loop de treinamento.
* `src/`: Scripts Python modulares.

## 📊 Resultados
* **Kappa Score:** 0.90
* **Acurácia:** 82%

## 🔗 Deploy
O modelo está em produção via FastAPI no Hugging Face: [Link do seu Space]
