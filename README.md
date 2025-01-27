# Fake News Detection

## Overview
The **Fake News Detection** project aims to combat the widespread issue of misinformation by developing a machine learning model that effectively classifies news articles as either "fake" or "real." The project utilizes robust natural language processing (NLP) techniques and multiple classification algorithms to ensure accurate results across diverse datasets.

---

## Features

- **Dataset Diversity**: A comprehensive dataset of labeled news articles covering various topics.
- **Text Preprocessing Pipeline**: Includes cleaning, stopword removal, and TF-IDF vectorization.
- **Model Evaluation**: Performance analysis using metrics like accuracy, precision, recall, and F1-score.
- **Manual Testing**: Test with real-world news snippets.
- **Top Performing Model**: Random Forest Classifier achieved the highest accuracy of 97.92%.

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

2. Create a virtual environment and install dependencies:
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

The dataset comprises a large collection of news articles labeled as either **fake** or **real**. The data underwent preprocessing to prepare it for machine learning tasks. Key preprocessing steps include:

1. Cleaning: Removal of HTML tags, special characters, and standardizing text to lowercase.
2. Stopword Removal: Eliminated common, non-informative words (e.g., "and", "the").
3. Vectorization: Converted text into numerical representations using **TF-IDF**.

---

## Models

Several machine learning models were implemented and evaluated:

1. **Logistic Regression**
   - Accuracy: 98%
   - F1-Score: 0.98
2. **Decision Tree Classifier**
   - Accuracy: 94.77%
   - F1-Score: 0.95
3. **Gradient Boosting Classifier**
   - Accuracy: 96.55%
   - F1-Score: 0.97
4. **Random Forest Classifier** (Best Performer)
   - Accuracy: 97.92%
   - F1-Score: 0.98

---

## Manual Testing

A testing function allows for real-world evaluation by taking user-input news articles. Results from manual testing confirmed the model's reliability in distinguishing fake from real news.

---

## Results

### Evaluation Metrics:

- **Accuracy**: Overall effectiveness of the model.
- **Precision**: Ability to identify only relevant instances.
- **Recall**: Capability of the model to retrieve all relevant instances.
- **F1-Score**: Harmonic mean of precision and recall.

---

## Future Enhancements

- **Advanced NLP Techniques**: Incorporate sentiment analysis and contextual embeddings for deeper language understanding.
- **Real-Time System**: Deploy the model in a real-time environment for live monitoring and detection.
- **Continuous Learning**: Enable adaptive updates with new data to stay current with trends in misinformation.

---

## Usage

1. To train and evaluate models, run the Jupyter Notebook in the `notebooks/` directory:
   ```bash
   jupyter notebook notebooks/Fake_News_Detection.ipynb
   ```

2. For manual testing, execute the script in the `tests/` directory:
   ```bash
   python tests/manual_test.py
   ```

---

## Contributing
Contributions are welcome! Please submit a pull request or raise an issue in the repository.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact
For any queries or feedback, please reach out to:

- **Name**: [Your Name]
- **Email**: [Your Email]
- **GitHub**: [Your GitHub Profile]

---

## Acknowledgments

- Inspiration for this project comes from the need to tackle misinformation in the digital age.
- Thanks to the open-source community for providing datasets and tools that made this project possible.
