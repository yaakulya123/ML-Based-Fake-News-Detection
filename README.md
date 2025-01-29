# Fake News Detection using Machine Learning

## Project Overview
Misinformation is a growing problem in the digital age. This project aims to **detect fake news articles** using various **Machine Learning algorithms**. A structured approach, including **data preprocessing, model evaluation, and real-world testing**, was implemented to ensure high accuracy.

The best-performing model, **Random Forest Classifier**, achieved **97.92% accuracy**, making it the most reliable choice for real-world application.


## Dataset
- The dataset consists of **news articles labeled as "fake" or "real"** from diverse sources.
- Preprocessing steps ensure **clean, structured text** for model training.
- **Vectorization Technique Used:** **TF-IDF (Term Frequency-Inverse Document Frequency)**



## Data Preprocessing
To prepare the text for ML models, the following steps were performed:

- **Text Cleaning** – Removing special characters, HTML tags, and converting text to lowercase.
- **Stopword Removal** – Eliminating common words like *"the"*, *"and"*, etc.
- **Vectorization** – Converting text into numerical features using **TF-IDF**, which highlights key terms contributing to fake news detection.



## Models Used
Multiple models were trained and evaluated to identify the best-performing one:

| Model                      | Accuracy  | F1-Score  |
|----------------------------|-----------|-----------|
| Logistic Regression        | 98%       | 0.98      |
| Decision Tree Classifier   | 94.77%    | 0.95      |
| Gradient Boosting          | 96.55%    | 0.97      |
| Random Forest Classifier   | **97.92%** | **Best!** |

**Best Model:** **Random Forest Classifier** – High precision, recall, and stability.


## Manual Testing
A **manual testing function** was implemented to allow **real-time testing** of new articles. Users can input a news snippet, and the model will classify it as **fake** or **real**.



## Evaluation Metrics
To ensure model reliability, these key metrics were used:

- **Accuracy** – Overall correctness of predictions.
- **Precision & Recall** – Balance between false positives and false negatives.
- **F1-Score** – Ensures a fair trade-off between precision and recall.



## Future Enhancements
- **Integrating advanced NLP techniques**, such as **sentiment analysis & contextual embeddings (BERT)**.
- **Deploying the model** as a **real-time API** for continuous monitoring of misinformation.
- **Enhancing feature selection** by incorporating **named entity recognition (NER)** for better classification.


## Setup & Usage

### 1. Install Dependencies
To install the necessary dependencies, run:
```bash
pip install -r requirements.txt
## Run the Model
Execute the following command to run the fake news detection model:

```bash
python fake_news_detection.py
```

## Manually Test a News Article
To manually classify a news article, use the following script:

```python
from model import predict_news

news_text = "Breaking: A major tech company announces a revolutionary AI breakthrough."
print(predict_news(news_text))
```

## Results & Reports

- **Classification Reports and Model Outputs** are available in the **documentation folder**.
- The documentation folder includes **detailed accuracy reports, confusion matrices, and manual testing results**.
- Performance metrics such as **precision, recall, and F1-score** are documented for all models.
