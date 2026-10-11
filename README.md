# NLP Text Classification & Spam Detection

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E.svg)](https://scikit-learn.org/)
[![NLTK](https://img.shields.io/badge/NLTK-3.8+-green.svg)](https://www.nltk.org/)
[![Internship](https://img.shields.io/badge/Maincrafts-Task%205-brightgreen.svg)](https://maincrafts.com/)

An end-to-end Natural Language Processing system implementing text cleaning, tokenization, lemmatization, TF-IDF n-gram feature extraction, and comparative text classification.

---

## Project Structure
- `AI_ML_Task5_NLP_Text_Classification.ipynb`: Complete preprocessing, vectorization, and model benchmark pipeline.
- `requirements.txt`: Python package dependencies.
- `README.md`: Technical methodology, comparative performance metrics, and usage instructions.

## Pipeline Architecture
1. **Text Preprocessing**: Lowercasing, regex URL/numeric removal, punctuation stripping, and WordNet lemmatization.
2. **Vectorization**: Sublinear TF-IDF feature extraction spanning unigrams and bigrams (`ngram_range=(1, 2)`).
3. **Model Evaluation**: Benchmark between Multinomial Naive Bayes, Logistic Regression, and Linear Support Vector Classifier using Stratified 5-Fold Cross-Validation.

## Performance Benchmark
| Model | Accuracy | Precision (Spam) | Recall (Spam) | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **LinearSVC** | **98.6%** | **0.99** | 0.91 | **0.95** |
| **MultinomialNB** | 98.2% | 0.94 | **0.93** | 0.93 |
| **Logistic Regression** | 97.9% | 0.98 | 0.86 | 0.92 |

## Setup & Execution
```bash
git clone [https://github.com/](https://github.com/)<your-username>/Maincrafts_AI_ML_Task5.git
cd Maincrafts_AI_ML_Task5
pip install -r requirements.txt
jupyter notebook AI_ML_Task5_NLP_Text_Classification.ipynb
