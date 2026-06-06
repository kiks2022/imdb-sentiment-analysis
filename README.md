# AnalystLab Africa — AI Internship Program
### Week 1 & 2: Natural Language Processing (NLP) — IMDB Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NLTK](https://img.shields.io/badge/NLTK-Text%20Processing-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## About This Project
This repository contains my work for **Week 1 & 2** of the AnalystLab Africa AI Internship Program.  
The goal was to explore **Natural Language Processing (NLP)** by cleaning and analyzing real-world movie reviews from the IMDB dataset.

The project focuses on preparing raw text data for machine learning by applying essential preprocessing techniques.

---

## Dataset
**IMDB Movie Reviews Dataset**

- 50,000 movie reviews
- 2 columns: `review`, `sentiment`
- Target column: `sentiment` (positive / negative)
- Balanced dataset (25,000 positive, 25,000 negative)
## Note on Dataset Size

The original IMDB dataset contains 50,000 reviews.

To keep this repository lightweight and within GitHub file size recommendations, a cleaned sample of 5,000 reviews (`cleaned_imdb_sample.csv`) is included instead of the full processed dataset.
---

## What I Did

### 1. Data Cleaning
| Problem | Solution |
|---|---|
| HTML tags like `<br />` | Removed using regex |
| Numbers and punctuation | Removed |
| Mixed case text | Converted to lowercase |
| Extra spaces | Stripped |

**Result:** Clean, structured text ready for analysis.

---

### 2. Tokenization
Converted each review into individual words using NLTK:

- Example:  
  `"I love this movie"` → `["i", "love", "this", "movie"]`

---

### 3. Stopword Removal
Removed common English words such as:
- "the"
- "is"
- "and"
- "a"

This helped focus on meaningful words only.

---

### 4. Word Frequency Analysis
Analyzed most common words in positive reviews.

Top words included:
- film
- movie
- great
- story
- love

---

### 5. Visualization
Created a bar chart showing the **Top 15 words in positive reviews**.

---

## Key Findings

### Dataset Balance
- Positive reviews: **50%**
- Negative reviews: **50%**
- Dataset is perfectly balanced for modeling

### Text Cleaning Impact
- Removing stopwords reduced noise significantly
- Average review length reduced by ~40–50%

### Language Insights
Positive reviews often contain words like:
- “great”
- “love”
- “best”
- “excellent”
- “story”

---

## Conclusion
This project demonstrates the importance of text preprocessing in NLP.

Raw text data is messy and unstructured. After cleaning, tokenization, and stopword removal, the dataset becomes suitable for machine learning models like sentiment classifiers.

---

## Files in This Repository

| File | Description |
|---|---|
| `IMDB_NLP.ipynb` | Main Jupyter notebook for analysis |
| `imdb_summary.txt` | Written summary of insights |
| `chart_top_words.png` | Top words visualization |
| `cleaned_imdb_sample.csv` | Sample cleaned dataset |
| `README.md` | Project documentation |

---

## Tools Used
- **Python 3.10**
- **Pandas** — data handling
- **NLTK** — natural language processing
- **Regex** — text cleaning
- **Matplotlib** — visualization
- **Google Colab** — development environment

---

## About
**Intern:** Adekoya Kikelomo Akorede  
**Program:** AnalystLab Africa AI Internship  
**Week:** 1 & 2 — AI Foundations & Data Preparation  
**Focus:** Natural Language Processing (NLP)
