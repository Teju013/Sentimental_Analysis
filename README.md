# Sentimental_Analysis
Emotion-based Sentiment Analysis using Transformer Models
📌 Overview
This project presents a comparative study of transformer-based models (BERT and DistilBERT) for emotion-based sentiment analysis.
The work investigates how large and small language models perform on tasks that require detecting emotions such as joy, anger, fear, sadness, surprise, and love in text.
Our findings indicate that while both models achieve good results, BERT outperforms DistilBERT in terms of accuracy and robustness for complex emotional sentiment tasks.
      
📊 Dataset
Dataset Used: EMOTION_LARGE.csv
Samples: 20,000 text samples
Labels:
*Joy
*Sadness
*Love
*Anger
*Fear
*Surprise
Challenge: The dataset is imbalanced (e.g., "joy" is frequent while "surprise" is rare).
Solution: Applied class-weighting to handle imbalance during training.

⚙️ Methodology
1.Data preprocessing & label mapping
2.Tokenization with Hugging Face Transformers
3.Fine-tuning BERT-base-cased and DistilBERT-base-cased models
4.Applied class-weight balancing
5.Evaluation using metrics: Accuracy, Precision, Recall, F1-score

🏗️ Architecture
<img width="721" height="349" alt="image" src="https://github.com/user-attachments/assets/e98f72c5-ee7b-450d-989f-3cb29001e009" />

📊 Results
The models were evaluated on the DAIR-AI Emotion Dataset (20,000 samples, 6 emotion labels) using Accuracy, Precision, Recall, and F1-score.
🔹 Performance Comparison
<img width="600" height="314" alt="image" src="https://github.com/user-attachments/assets/2e811068-e6fe-495d-b75b-f98da128a9e6" />
<img width="683" height="435" alt="image" src="https://github.com/user-attachments/assets/3de50cea-b357-4314-a69c-1c820455fca7" />
<img width="697" height="427" alt="image" src="https://github.com/user-attachments/assets/a622ce56-b43f-4ead-8e35-77a2283f60aa" />
<img width="709" height="421" alt="image" src="https://github.com/user-attachments/assets/b371e0ef-f4a2-4418-9f45-bfc133f487df" />

🔮 Future Work
*Extend to aspect-level sentiment analysis (e.g., political protests, product reviews)
*Build ensemble prediction models combining multiple transformers
*Use larger and more diverse datasets for better generalization
