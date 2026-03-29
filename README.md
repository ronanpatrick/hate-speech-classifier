# Filipino Hate Speech Classifier (NLP)

> **Objective:** To develop a robust Natural Language Processing (NLP) pipeline capable of classifying text as hate speech within the context of the Filipino language, comparing the efficacy of multiple machine learning algorithms.

## Overview
This repository contains an end-to-end NLP case study focused on text classification. Handling localized dialects and slang requires specific preprocessing and feature extraction techniques. This project utilizes TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to process the text data before training and evaluating multiple classification models to determine the most accurate approach for identifying toxic online content.

**A comprehensive breakdown of model performance, metrics, and difficult-to-classify samples is available in the included PDF Evaluation Report.**

## Dataset
* **Structure:** The dataset is pre-split into `train.csv`, `test.csv`, and `valid.csv` for proper model training and validation.
* **Domain:** Filipino text snippets labeled for hate speech classification.

## Repository Structure
*  **`Model_Evaluation_Report.pdf`**: The formal documentation detailing the methodology, comparative analysis of the models, and insights into misclassified samples.
*  **`Filipino_Hate_Speech_Classifier.ipynb`**: The core Jupyter Notebook containing the data ingestion, TF-IDF vectorization, model training, and metric evaluation.
*  **Data Files**: `train.csv`, `test.csv`, and `valid.csv`.

## Tech Stack
* **Language:** Python
* **Natural Language Processing:** Scikit-Learn (`TfidfVectorizer`, `CountVectorizer`)
* **Machine Learning Models:** Scikit-Learn (`LinearSVC`, `LogisticRegression`, `RandomForestClassifier`), XGBoost (`XGBClassifier`)
* **Data Manipulation & Viz:** Pandas, NumPy, Matplotlib, Seaborn

## How to Run the Notebook

### Option 1: Run in Cloud (Recommended)
You can view and execute the code instantly in your browser via Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ronanpatrick/hate-speech-classifier/blob/main/Hate_Speech_Classifier.ipynb)

*(Note: If running in Colab, please ensure you upload `train.csv`, `test.csv`, and `valid.csv` to your session storage first).*

### Option 2: Run Locally
1. Clone this repository: `git clone https://github.com/ronanpatrick/filipino-hate-speech-classifier.git`
2. Install the required libraries: `pip install pandas numpy scikit-learn xgboost matplotlib seaborn`
3. Open the `.ipynb` file in Jupyter Notebook or VS Code and execute the cells.
