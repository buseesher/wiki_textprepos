# 🧠 Wiki Text Preprocessing & Visualization

This project demonstrates basic text preprocessing techniques on a Wikipedia dataset, including case normalization, punctuation and number removal, stopword filtering, rare word filtering, lemmatization, and basic visualizations such as bar plots and word clouds.

---

## 📂 Project Overview

**Filename**: `wiki_textpreprocessing_visualization.py`  
**Dataset**: `datasets/wiki_data.csv`  
**Subset Used**: First 2000 records from the full dataset

---

## 🛠️ Features

- ✅ Text cleaning (case folding, punctuation & number removal)
- ✅ Stopword and rare word filtering
- ✅ Lemmatization using `TextBlob`
- 📊 Word frequency bar plot (TF)
- ☁️ Word cloud generation
- 📦 All preprocessing steps are encapsulated in a single function: `wiki_preprocess`

---

## 🔍 Requirements

Make sure you have the following Python libraries installed:

```bash
 pip install pandas matplotlib wordcloud nltk textblob
  ```

You may also need to download NLTK stopwords:
```bash
 import nltk
nltk.download('stopwords')
  ```
---

## ▶️ How to Run

1.Ensure the file wiki_data.csv is placed under:
Modül_8_Dogal_Dil_İşleme/datasets/wiki_data.csv

2.Run the script:
```bash
 python wiki_textpreprocessing_visualization.py
  ```
3.Optional: Enable visualizations from the function:
```bash
 wiki_preprocess(df["text"], Barplot=True, Wordcloud=True)
  ```
---

## 🧪 Function: wiki_preprocess()

*Parameters:*

-text: Pandas Series containing text data

-Barplot: Set to True to display most frequent words (TF > 2000)

-Wordcloud: Set to True to generate a word cloud

*Returns:*

-Cleaned Pandas Series of preprocessed text data

---

## 📈 Sample Visualizations
-Most frequent words (bar plot)

-Word cloud of top 100 most common words (after preprocessing)
