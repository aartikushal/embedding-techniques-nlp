# 📘 Embedding Assignment - NLP Project

## 📌 Objective
This assignment explores different **word embedding techniques** for Natural Language Processing (NLP) tasks. The goal is to transform raw text into meaningful numerical representations using:

- TF-IDF  
- Word2Vec  
- GloVe  
- FastText  

Each method is implemented, compared, and optionally used in downstream tasks like **classification** or **clustering**.

---

## 🧰 Requirements
Install dependencies:



## 📂 Project Structure

embedding-assignment/
├── data/
│   └── corpus.txt             # Text corpus for training embeddings
├── embeddings/
│   ├── glove.6B.100d.txt      # Pre-trained GloVe vectors (downloaded)
│   └── custom_vectors.txt     # Trained Word2Vec or FastText vectors (optional)
├── notebook.ipynb             # Main analysis notebook
├── glove_utils.py             # GloVe loading utility
├── README.md                  # This file


## 🔍 Methods Implemented
1️⃣ TF-IDF (Term Frequency-Inverse Document Frequency)

Vectorizes text using frequency-based weighting.

Implemented using sklearn.feature_extraction.text.TfidfVectorizer.

2️⃣ Word2Vec

Trains word embeddings using the Skip-gram or CBOW model.

Implemented using gensim.models.Word2Vec.

3️⃣ GloVe

Uses pre-trained vectors (glove.6B.100d.txt).

Mapped via a tokenizer's word index to form an embedding matrix.

Optional: Custom GloVe training.

4️⃣ FastText

Embeddings from subwords using gensim.models.FastText.

Useful for out-of-vocabulary (OOV) words.

## 📥 How to Use
Pre-trained GloVe

Download GloVe vectors: GloVe Project

Place glove.6B.100d.txt into the embeddings/ folder.

Load embeddings using:
from glove_utils import load_glove_embeddings

glove_dict = load_glove_embeddings("embeddings/glove.6B.100d.txt")

from glove_utils import load_glove_embeddings

glove_dict = load_glove_embeddings("embeddings/glove.6B.100d.txt")


## 📚 References

GloVe Project

Gensim Documentation

TF-IDF – scikit-learn

## 👩‍💻 Author

Name: Aarti Potdar
Course: NLP / Machine Learning Assignment


This version is **fully formatted for GitHub**, copy-paste ready, and includes headings, code blocks, tables, and links.  

If you want, I can also **add badges for Python, Jupyter Notebook, and NLP** to make it look professional on GitHub. Do you want me to do that?
