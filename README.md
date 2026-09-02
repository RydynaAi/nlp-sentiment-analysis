# nlp-sentiment-analysis
End-to-end NLP sentiment analysis pipeline built from scratch in Python — custom text preprocessing (tokenization, stopword removal, Porter stemming) and a VADER-based sentiment scoring engine, with visualizations and result interpretation.
<div align="center">

# 💬 NLP Sentiment Analysis

### End-to-end sentiment analysis pipeline built from scratch in Python

<p>
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python" alt="Python"/>
  <img src="https://img.shields.io/badge/pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="pandas"/>
  <img src="https://img.shields.io/badge/VADER-Sentiment%20Engine-orange" alt="VADER"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white" alt="Jupyter"/>
</p>

</div>

---

## 📖 About

<p>
This project implements a complete <b>sentiment analysis pipeline</b> from scratch — without relying on
external NLP libraries for the core logic. Both the text preprocessing steps (inspired by NLTK) and the
<b>VADER</b> sentiment scoring engine are implemented manually in pure Python, using a custom dataset of
120 text samples (reviews, tweets, and comments).
</p>

<table>
<tr>
  <td><b>📦 Dataset</b></td>
  <td>120 English text samples (reviews, tweets, comments)</td>
</tr>
<tr>
  <td><b>🧹 Preprocessing</b></td>
  <td>Link removal, tokenization, lowercasing, stopword removal, punctuation removal, Porter stemming</td>
</tr>
<tr>
  <td><b>🧠 Sentiment Engine</b></td>
  <td>Custom VADER implementation (neg, neu, pos, compound)</td>
</tr>
<tr>
  <td><b>📊 Visualizations</b></td>
  <td>Bar chart, pie chart, compound score distribution, source breakdown</td>
</tr>
</table>

---

## ✨ Features

<ul>
  <li>🧹 Full text preprocessing pipeline implemented from scratch (no external NLP library calls)</li>
  <li>🌱 Custom Porter Stemmer built in pure Python</li>
  <li>🧠 Custom VADER-style lexicon and scoring function (neg / neu / pos / compound)</li>
  <li>🏷️ Automatic classification into Positive, Neutral, or Negative</li>
  <li>📊 Multiple visualizations: bar chart, pie chart, and stacked bar chart by source</li>
  <li>📝 Automated interpretation summary of the results</li>
  <li>💾 Exports processed results to a CSV file</li>
</ul>

---

## 🗂️ Project Structure

<pre>
nlp-sentiment-analysis/
├── NLP_Sentiment_Analysis.ipynb   # Main notebook (Steps 1–6)
├── sentiment_dataset.csv          # Input dataset (text, source)
├── processed_results.csv          # Generated after running the notebook
├── requirements.txt
└── README.md
</pre>

---

## 🛠️ Tech Stack

<table>
<tr><th>Layer</th><th>Technology</th></tr>
<tr><td>Data Handling</td><td>pandas, numpy</td></tr>
<tr><td>Text Processing</td><td>Custom Python (re, string) — Porter Stemmer, stopword filter</td></tr>
<tr><td>Sentiment Scoring</td><td>Custom VADER-style lexicon and scorer</td></tr>
<tr><td>Visualization</td><td>matplotlib</td></tr>
<tr><td>Environment</td><td>Jupyter Notebook, Python 3.11</td></tr>
</table>

---

## ⚡ Getting Started

### Prerequisites
- Python 3.11

### 1. Clone the repository
<pre>
git clone https://github.com/&lt;your-username&gt;/nlp-sentiment-analysis.git
cd nlp-sentiment-analysis
</pre>

### 2. Install dependencies
<pre>
pip install -r requirements.txt
</pre>

### 3. Run the notebook
<pre>
jupyter notebook NLP_Sentiment_Analysis.ipynb
</pre>
<p>Run all cells from top to bottom — the dataset (<code>sentiment_dataset.csv</code>) is already included.</p>

---

## 📊 Pipeline Overview

<table>
<tr><th>Step</th><th>Description</th></tr>
<tr><td>1. Imports & Configuration</td><td>Load required libraries</td></tr>
<tr><td>2. Dataset Loading</td><td>Load and inspect the 120-sample dataset</td></tr>
<tr><td>3. Preprocessing</td><td>Clean and normalize text using a custom NLTK-style pipeline</td></tr>
<tr><td>4. Sentiment Analysis</td><td>Score each sample with the custom VADER engine</td></tr>
<tr><td>5. Visualization</td><td>Plot sentiment distribution and breakdown by source</td></tr>
<tr><td>6. Interpretation</td><td>Summarize dominant sentiment and key observations</td></tr>
</table>

---

## 📈 Example Output

<p>
The notebook classifies each sample as <b>Positive</b>, <b>Neutral</b>, or <b>Negative</b> based on its
compound score (≥ 0.05 → Positive, ≤ −0.05 → Negative, otherwise Neutral), then visualizes the distribution
across the full dataset and by source (review / tweet / comment).
</p>

---

## 👤 Author

<p>Rudyna Al-Qarni</p>
