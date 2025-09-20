# Sentimental_Analysis

Emotion-based Sentiment Analysis using Transformer Models (BERT & DistilBERT)

📌 Overview

This project evaluates the performance of transformer-based language models BERT and DistilBERT for emotion detection in sentiment analysis.
The task focuses on identifying six emotions from text data:

Joy

Sadness

Anger

Fear

Love

Surprise

The study compares the performance of large (BERT) and smaller (DistilBERT) transformer architectures on an imbalanced dataset using fine-tuning and weighting strategies.

📊 Dataset

Dataset Used: DAIR-AI Emotion Dataset

Size: 20,000 samples

Labels: Joy, Sadness, Anger, Fear, Love, Surprise

Train / Validation / Test Split: 70% / 20% / 10%

Challenge: Imbalanced class distribution (e.g., Joy & Sadness more frequent, Surprise & Love less frequent)

⚙️ Methodology

1.Data Preprocessing

      Label mapping

      Tokenization using Hugging Face Transformers

      Handling class imbalance via inverse frequency class weighting

2.Model Training

      Pretrained Models: bert-base-cased and distilbert-base-cased

      Hyperparameters:

            Epochs: 3

            Batch Size: 8

            Learning Rate: 2e-5

            Weight Decay: 0.01

3.Evaluation Metrics

      Accuracy

      Precision

      Recall

      F1-Score

      Confusion Matrix

📈 Results

Before Handling Imbalance

<img width="979" height="220" alt="image" src="https://github.com/user-attachments/assets/23ae480a-79fe-4227-9de3-dc95f596453c" />

After Handling Imbalance

<img width="979" height="219" alt="image" src="https://github.com/user-attachments/assets/10f7069c-09b6-4300-a385-961fb2831456" />

🔹 Key Observations:

BERT consistently outperforms DistilBERT overall.

DistilBERT shows competitive results and sometimes surpasses BERT on minority labels with fewer samples.

Weighted loss significantly improved both models’ performance on imbalanced data.

📜 Conclusion

BERT achieved the best overall accuracy (94.65%) after class imbalance handling.

DistilBERT, while smaller and faster, achieved near-competitive performance (94.35%) and sometimes outperformed BERT on minority classes.

Weighted loss functions are effective in addressing dataset imbalance for emotion classification tasks.
