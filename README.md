# 📰 T5 Headline Generation

This project fine-tunes a **T5-small transformer model** to generate news headlines from article text using abstractive summarization.

---

## 📌 Overview

* Task: Headline Generation (Text → Headline)
* Model: `t5-small`
* Approach: Transfer Learning (Fine-tuning)
* Dataset: ~4,500 news articles (text + headline)

---

## ⚙️ Model Configuration

| Parameter        | Value    |
| ---------------- | -------- |
| Model            | T5-small |
| Learning Rate    | 2e-5     |
| Epochs           | 3        |
| Batch Size       | 8        |
| Weight Decay     | 0.01     |
| Train/Test Split | 80 / 20  |

---

## 🧪 Evaluation Results

### ROUGE (Lexical Similarity)

| Metric     | Score  |
| ---------- | ------ |
| ROUGE-1    | 0.3336 |
| ROUGE-2    | 0.1740 |
| ROUGE-L    | 0.3187 |
| ROUGE-Lsum | 0.3201 |

### BERTScore (Semantic Similarity)

| Metric    | Score  |
| --------- | ------ |
| Precision | 0.8810 |
| Recall    | 0.8840 |
| F1 Score  | 0.8824 |

**Summary:**

* Strong **semantic understanding** (high BERTScore)
* Moderate **word-level overlap** (ROUGE) due to abstractive generation

---
