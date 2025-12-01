# VisusAI - Deep Learning Training Pipeline 🧠

Repositório dedicado à engenharia e treinamento do modelo de Visão Computacional para detecção de Retinopatia Diabética.

## 🔬 O Modelo
Utilizei a **EfficientNet-B4** (PyTorch Image Models - timm) com Transfer Learning.

## ⚙️ Pipeline de Treinamento
Este projeto resolve desafios comuns de datasets médicos:

1.  **Pré-processamento (CLAHE):** Aplicação de contraste adaptativo para realçar microaneurismas.
2.  **Resolução:** Input de 512x512px (acima do padrão 224px).
3.  **Balanceamento:** Uso de `WeightedRandomSampler` para corrigir o desbalanceamento severo entre classes "Normal" e "Proliferativa".

## 📚 Dataset 

* **O dataset aptos2019 foi utilizado para treinar o modelo
* **Disponível no Kaggle ou via [https://www.kaggle.com/c/aptos2019-blindness-detection]

## 📊 Resultados
* **Kappa Score:** 0.90
* **Acurácia:** 80%

<img width="771" height="176" alt="image" src="https://github.com/user-attachments/assets/82987635-4e5a-498f-b7b8-5d36cab1e3de" />

* ** Exemplo de Inferência

<img width="619" height="661" alt="image" src="https://github.com/user-attachments/assets/10a8a755-b4ed-4a5a-ba62-2728dc280067" />



## 🔗 Deploy
O modelo está em produção via FastAPI no Hugging Face: [Link do seu Space]

