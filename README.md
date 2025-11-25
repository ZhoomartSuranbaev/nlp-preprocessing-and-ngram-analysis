# 📘 **NLP Text Cleaning and N-grams**

This project demonstrates a complete NLP preprocessing pipeline applied to raw English text collected from Wikipedia. It covers text extraction, cleaning, tokenization, lemmatization, stopword removal, and N-gram analysis (unigrams, bigrams, trigrams).
All experiments were performed in Google Colab.

---

## 🚀 **Project Goals**

* Collect raw English text from Wikipedia
* Clean and normalize the text
* Perform tokenization and lemmatization
* Remove English stopwords
* Generate N-grams (1–3)
* Visualize the most frequent N-grams
* Build a simple and reproducible NLP preprocessing workflow

---

## 📂 **Project Structure**

```
project/
│
├── NLP_Text_Cleaning.ipynb        # Main Google Colab notebook
├── README.md                      # Project documentation
└── requirements.txt (optional)    # Python dependencies
```

---

## 📊 **Dataset**

The raw dataset is collected directly from Wikipedia using the `wikipedia` Python package.

**Wikipedia pages used:**

* *Artificial intelligence*
* *Machine learning*
* *Data science*

The text is split into sentences and stored in a pandas DataFrame.

---

## 🧹 **Text Cleaning Steps**

Each text entry goes through the following preprocessing pipeline:

1. Lowercasing
2. Removing punctuation
3. Removing numbers
4. Tokenization
5. Removing stopwords
6. Lemmatization
7. Returning clean tokens

Implemented using:

* `nltk.word_tokenize`
* `nltk.corpus.stopwords`
* `WordNetLemmatizer`

---

## 🔠 **N-gram Generation**

Custom function `get_ngrams(tokens_list, n)` generates:

* **Unigrams (n=1)**
* **Bigrams (n=2)**
* **Trigrams (n=3)**

Frequencies are computed using:

```python
from collections import Counter
```

---

## 📈 **Visualization**

The top 10 most frequent:

* Unigrams
* Bigrams
* Trigrams

are visualized using **matplotlib** bar charts.

---

## 🛠 **Dependencies**

Install all required packages:

```bash
pip install pandas numpy nltk matplotlib wikipedia
```

Download NLTK data inside the notebook:

```python
nltk.download('punkt')
nltk.download('punkt_tab')
nltk.download('stopwords')
nltk.download('wordnet')
```

---

## ▶️ **How to Run**

Open the notebook in Google Colab:

1. Clone the repository
2. Open `.ipynb` notebook
3. Run all cells
4. Review the output DataFrames and visualizations

---

## 📌 **Result**

The project produces:

✔ A cleaned dataset with tokenized and lemmatized text
✔ Unigram, bigram, and trigram frequency lists
✔ Visual charts of top N-grams
✔ A reusable NLP preprocessing pipeline

---

## 📜 **License**

This project is open-source and available under the MIT License.

---

## 🤝 **Contributions**

Pull requests and improvements are welcome.
Feel free to fork the project and experiment with other datasets or NLP methods.
