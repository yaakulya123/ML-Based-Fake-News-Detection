# Fake News Detection

## Overview
This **Fake News Detection** project was done as part of my academic work to tackle the widespread issue of misinformation. The goal was to build a machine learning model that classifies news articles as either "fake" or "real." Working on this project was a great learning experience, and it helped me explore natural language processing (NLP) techniques and classification models.

---

## Features

- **Diverse Dataset**: The dataset I used has labeled news articles across different topics, making the model adaptable.
- **Preprocessing Pipeline**: I cleaned, vectorized, and prepared text data for machine learning.
- **Model Comparison**: I evaluated different algorithms based on their performance.
- **Interactive Testing**: Added a manual testing feature to check the model on real-world inputs.
- **Best Model**: The Random Forest Classifier achieved the highest accuracy of 97.92%.

---

## Project Structure

```plaintext
Fake-News-Detection/
├── data/               # Dataset files
├── notebooks/          # Jupyter notebooks for model development and evaluation
├── src/                # Source code for preprocessing, training, and evaluation
├── tests/              # Manual testing scripts
├── images/             # Visualizations and classification reports
├── README.md           # Project documentation (this file)
```

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Fake-News-Detection.git
   cd Fake-News-Detection
   ```

2. Set up a virtual environment and install the required packages:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Install Jupyter Notebook (optional):
   ```bash
   pip install notebook
   ```

---

## Dataset

The dataset contains a collection of news articles labeled as **fake** or **real.** Before training, I applied preprocessing techniques like:

1. Cleaning: Removed HTML tags, special characters, and standardized text to lowercase.
2. Stopword Removal: Removed common words (like "and", "the") that don't add value.
3. Vectorization: Converted text into numbers using **TF-IDF**, highlighting important words.

---

## Models

I tried out several machine learning models to find the best one:

1. **Logistic Regression**
   - Accuracy: 98%
   - F1-Score: 0.98
2. **Decision Tree Classifier**
   - Accuracy: 94.77%
   - F1-Score: 0.95
3. **Gradient Boosting Classifier**
   - Accuracy: 96.55%
   - F1-Score: 0.97
4. **Random Forest Classifier** (Best Model)
   - Accuracy: 97.92%
   - F1-Score: 0.98

---

## Manual Testing

I also added a manual testing script where you can input news articles and see the model's predictions. This feature makes it easy to test the project in a real-world context.

---

## Results

### Evaluation Metrics:

- **Logistic Regression**: Accuracy = 98%, F1-Score = 0.98
- **Decision Tree Classifier**: Accuracy = 94.77%, F1-Score = 0.95
- **Gradient Boosting Classifier**: Accuracy = 96.55%, F1-Score = 0.97
- **Random Forest Classifier**: Accuracy = 97.92%, F1-Score = 0.98

---

## Future Enhancements

- **Advanced NLP Techniques**: I plan to explore sentiment analysis and embeddings for better accuracy.
- **Real-Time System**: Would love to deploy this as a live application for detecting fake news.
- **Adaptive Learning**: Updating the model with new data to handle evolving trends in misinformation.

---

## Usage

1. Open the Jupyter Notebook in the `notebooks/` folder to train and evaluate models:
   ```bash
   jupyter notebook notebooks/Fake_News_Detection.ipynb
   ```

2. Test news articles manually using the script in the `tests/` directory:
   ```bash
   python tests/manual_test.py
   ```

---

## Contributing
If you find this interesting or have suggestions for improvement, feel free to contribute or share your thoughts!
