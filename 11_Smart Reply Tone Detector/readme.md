# Tone Analyzer & Intelligent Auto-Reply System

An intelligent Natural Language Processing (NLP) system built with Python, Scikit-Learn, and NLTK to detect the underlying emotional tone of text messages and generate context-appropriate, polite, and professional auto-replies. 

This application classifies incoming text into four distinct tones:
*   **Polite** 😊
*   **Neutral** 😐
*   **Passive-Aggressive** 😒
*   **Rude (including explicit or informal frustration)** 🤬

---

## 🚀 Features

*   **Custom Text Preprocessing Pipeline:** Tokenization, lowercasing, punctuation removal, stopword exclusion, and stemming via NLTK's `PorterStemmer`.
*   **Machine Learning Classifier:** Feature extraction using `TfidfVectorizer` (Term Frequency-Inverse Document Frequency) paired with a robust `LogisticRegression` model.
*   **Explicit Content Handling:** Enhanced training dataset specifically addresses edge cases, ensuring profanities and rude slang are classified accurately.
*   **Interactive Interface:** A clean command-line interface to test sentences interactively and view the recommended professional response instantly.

---

## 🛠️ Tech Stack

*   **Language:** Python 3
*   **Machine Learning:** Scikit-Learn
*   **NLP Processing:** NLTK (Natural Language Toolkit)
*   **Data Manipulation:** Pandas

---

## 📦 Setup & Installation

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/tone-analyzer-autoreply.git
    cd tone-analyzer-autoreply
    ```

2.  **Install Required Libraries:**
    ```bash
    pip install nltk scikit-learn pandas
    ```

3.  **Download NLTK Corpus Data:**
    Open your Python terminal or add this to your initialization script:
    ```python
    import nltk
    nltk.download('stopwords')
    ```

---

## 💻 How to Run the App

Run the primary python script or execute the interactive notebook cells. When prompted, type your message:

```python
# Run the main interactive prompt
user_input = input("Enter a message to analyze: ")
get_smart_reply(user_input)
Sample Session Output
==================================================
Original Message: you are a shit
Detected Tone:    RUDE
Suggested Reply:  I understand your concern. Could you please explain what needs to be corrected?
==================================================
🧠 System Architecture & Methodology
Text Normalization: Lowercases text and strips punctuation using string translation tables.
Stemming: Reduces words to their word stems (e.g., "careless" and "carelessness" mapped to "care") so that morphological variations share features.
TF-IDF Vectorization: Converts preprocessed text sequences into mathematical vectors representing word importance relative to the corpus.
Classification: A Logistic Regression model predicts one of the four classes based on maximum likelihood estimation probabilities.
Polite Mapping Engine: Maps predicted classes to tailored replies designed to de-escalate workplace conflict.
