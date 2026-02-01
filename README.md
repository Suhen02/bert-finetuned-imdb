# BERT Fine‑Tuning on IMDb Sentiment Dataset

##  Overview
This repository contains a Jupyter/Colab notebook that demonstrates how to fine‑tune **BERT** for sentiment analysis on the IMDb movie reviews dataset.  
The notebook walks through:
- Loading and preprocessing the IMDb dataset  
- Tokenizing text with Hugging Face `transformers`  
- Fine‑tuning BERT for binary classification (positive vs negative reviews)  
- Evaluating the model’s performance  

---
## 🔗 Model on Hugging Face Hub
You can access and use the fine‑tuned model here:  
👉 [Suhen/bert-finetuned-imdb](https://huggingface.co/Suhen/bert-finetuned-imdb)

To load it directly in Python:
```python
from transformers import pipeline

sentiment_model = pipeline("sentiment-analysis", model="Suhen/bert-finetuned-imdb")
print(sentiment_model("I loved this movie!"))
```

---
## How to Use

### 1. Clone the repo
```bash
git clone  https://github.com/Suhen02/bert-finetuned-imdb.git
cd bert-finetuned-imdb
```
### 2.Install dependencies
```bash
pip install transformers datasets torch scikit-learn
```
