# 🧭 Intent-Router-Engine

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Latest-orange.svg)
![NLTK](https://img.shields.io/badge/NLTK-NLP-green.svg)

**Intent-Router-Engine** is a supervised machine learning pipeline built to accurately classify natural language queries into actionable intents. By leveraging robust text pre-processing and predictive modeling, this engine serves as the foundational routing layer for AI assistants, chatbots, and automated support systems.

## 📌 Project Overview
Modern AI systems require a reliable method to understand *what* a user wants before generating a response or executing a command. This project processes raw text inputs, cleans the data using natural language processing (NLP) techniques, and routes the query to the correct predefined category using supervised classification models.

### 🚀 Key Features
* **Comprehensive Pre-processing:** Automated text normalization pipeline including tokenization, stop-word filtering, punctuation removal, and stemming/lemmatization using `NLTK` and `Regex`.
* **Multi-Model Pipeline:** Implements and compares multiple predictive models (e.g., Naive Bayes, Support Vector Machines, Random Forest) to find the optimal classifier for the chosen dataset.
* **Automated Hyperparameter Tuning:** Integrates `GridSearchCV` / `RandomizedSearchCV` to systematically discover the best parameters for maximum routing accuracy.
* **Robust Evaluation:** Outputs clear evaluation metrics including accuracy, precision, recall, F1-scores, and confusion matrices to critically analyze model performance.

## 📊 Dataset
This engine is currently trained and evaluated on the **[Insert Dataset Name Here, e.g., SNIPS / MASSIVE / CLINC150]** dataset. 
* **Domain:** [e.g., General Voice Assistant Commands]
* **Total Instances:** [e.g., ~16,000]
* **Distinct Intents:** [e.g., 7 core intents]

*(Detailed Exploratory Data Analysis (EDA) can be found in the accompanying Jupyter Notebooks).*

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **NLP Processing:** `nltk`, `textblob`, `re`
* **Machine Learning:** `scikit-learn`
* **Visualization:** `matplotlib`, `seaborn` (for EDA and Confusion Matrices)

## 📂 Repository Structure
```text
├── data/                   # Raw and processed dataset files (ignored in git)
├── notebooks/              # Jupyter notebooks for EDA and model experiments
├── src/                    # Source code for the engine
│   ├── preprocess.py       # Text normalization and cleaning functions
│   ├── train.py            # Model training and hyperparameter tuning logic
│   └── evaluate.py         # Scoring and visualization scripts
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation