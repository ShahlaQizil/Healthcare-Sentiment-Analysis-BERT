# Healthcare Sentiment Analysis using BERT

## 📌 Project Overview
This project focuses on fine-tuning a pre-trained **BERT (Bidirectional Encoder Representations from Transformers)** model to classify the sentiment of patient reviews in the healthcare industry. 

The goal is to automatically categorize feedback as **Positive**, **Neutral**, or **Negative** to help healthcare providers improve their services.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Hugging Face (Transformers), PyTorch, Pandas, Scikit-learn
- **Platform:** Google Colab (GPU: T4)

## 🚀 Key Features & Workflow
Based on the **Microsoft AI and ML Engineering** professional certificate curriculum:
1. [cite_start]**Data Preprocessing:** Handled missing values and noisy text (URLs, special characters)[cite: 17, 19].
2. [cite_start]**Text Normalization:** Standardized text to lowercase and removed unnecessary whitespaces[cite: 20, 48].
3. [cite_start]**Tokenization:** Used `AutoTokenizer` from BERT-base-uncased to convert text into tensors[cite: 18, 67].
4. [cite_start]**Fine-Tuning:** Specialized a pre-trained LLM for sequence classification tasks[cite: 1, 101].
5. [cite_start]**Evaluation:** Measured performance using Accuracy and F1-Score[cite: 120, 136].

## 📊 Dataset
The model was trained on a sample dataset of hospital reviews. 
*Example inputs:*
- "The staff was very kind..." -> **Positive**
- "The waiting time was too long..." -> **Negative**

## 📥 How to Use
1. Clone this repository.
2. Open `BERT_Sentiment_Analysis.ipynb` in Google Colab.
3. Upload your own `hospital_reviews.csv` when prompted.
4. Run all cells to see the fine-tuning process and evaluation results.

## 📜 Acknowledgments
This project was developed as part of the **"Building Intelligent Troubleshooting Agents"** course, which is the 3rd course in the **Microsoft AI and ML Engineering Professional Certificate** on Coursera.

## 📈 Performance Results
After fine-tuning the BERT model on the healthcare dataset, the model achieved perfect scores on the test set:
- **Final Accuracy:** 1.00 (100%)
- **Final F1-Score:** 1.00

### Training Summary:
- **Total Training Epochs:** 3
- **Training Loss:** 1.0872
- **Hardware used:** Google Colab T4 GPU
- **Framework:** Hugging Face Trainer API

*Note: The 100% accuracy is due to the small size of the sample dataset. In a real-world scenario with thousands of varied reviews, these metrics would provide a more generalized reflection of the model's power.*
