# ITAI2373-NewsBot-Midterm
# NewsBot Intelligence System 🤖📰

## Project Overview
The NewsBot Intelligence System is an end-to-end Natural Language Processing (NLP) pipeline designed to automatically process, categorize, and extract actionable business insights from raw news articles. Built as a comprehensive data science project, the system ingests unstructured text and outputs structured intelligence, enabling automated media monitoring, content routing, and sentiment tracking.

## Technical Pipeline
This system integrates 8 distinct NLP modules into a single, cohesive workflow:
1. **Text Preprocessing:** Cleans HTML, URLs, and special characters while applying tokenization, stop-word removal, and lemmatization using `NLTK` and `Regex`.
2. **Feature Extraction:** Utilizes `scikit-learn`'s `TfidfVectorizer` to identify distinctive keywords per category.
3. **Grammatical Pattern Analysis:** Applies Part-of-Speech (POS) tagging to detect varying writing styles (e.g., proper noun density in Business vs. action verbs in Politics).
4. **Syntax & Semantics:** Extracts sentence structure and Subject-Verb-Object relationships using `spaCy` dependency parsing.
5. **Sentiment Analysis:** Scores emotional tone utilizing the `VADER` sentiment analyzer to gauge public perception.
6. **Multi-Class Text Classification:** Trains and tunes machine learning algorithms (Naive Bayes, Logistic Regression, SVM) to predict news categories. Handles class imbalance and includes hyperparameter tuning. 
7. **Named Entity Recognition (NER):** Extracts critical facts (PERSON, ORG, GPE, MONEY, DATE) to map entity relationships across the corpus.
8. **Actionable Insights:** Translates technical model outputs into business recommendations.

## Dataset & Performance
* **Dataset:** 1,490 curated articles from the BBC News dataset.
* **Categories:** Business, Entertainment, Politics, Sport, and Tech.
* **Model Accuracy:** **97.32%** (Optimized Naive Bayes with scaled length features).
* **Entity Extraction:** Identified over **44,900** named entities.

## Business Value
This pipeline demonstrates how media organizations and financial firms can automate content management. By pairing high-accuracy classification with NER and sentiment tracking, organizations can automatically route daily content to appropriate editorial desks, track brand sentiment over time, and map entity co-occurrences without manual human intervention.

## Repository Structure
* `Midterm_NewsBot_Intelligence_System_student.ipynb`: The complete, runnable Jupyter Notebook containing the end-to-end Python pipeline, analysis, and visualizations.
* `newsbot_dataset.csv`: The cleaned and formatted dataset used to train and test the models.
* `README.md`: Project overview and documentation.

## Author
* **Dana Bolden** - *Lead Developer*
