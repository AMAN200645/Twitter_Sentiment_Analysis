# 🐦 Twitter Sentiment Analysis App

This project is a deep learning-based sentiment analysis tool that uses an LSTM model to classify Twitter text into **Positive**, **Neutral**, or **Negative** sentiments. The app is built with TensorFlow and deployed via a simple Streamlit interface for real-time predictions.

---

## 📁 Project Structure

```
twitter-sentiment-app/
├── Twitter_Data.csv           # Dataset for training
├── sentiment_model.h5         # Trained LSTM model
├── tokenizer.joblib           # Saved tokenizer
├── twitter_sentiment_main.py  # Model training script
├── twitter_sentiment_app.py   # Streamlit web application
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
```

---

## 📌 Features

- LSTM-based deep learning model using Keras
- Real-time sentiment prediction with Streamlit
- Preprocessing and tokenization with Keras Tokenizer
- Supports three sentiment classes: Negative, Neutral, Positive

---

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/twitter-sentiment-app.git
cd twitter-sentiment-app
```

### 2. Create Virtual Environment (Optional)

```bash
python -m venv venv
# For Windows:
venv\Scripts\activate
# For Unix/Mac:
source venv/bin/activate
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

---

## 🚀 Running the App

After installing all dependencies, start the Streamlit app with:

```bash
streamlit run twitter_sentiment_app.py
```

Open the local URL (http://localhost:8501/) in your browser to access the app.

---

## 🏋️ Training the Model (Optional)

If you want to train the model again using your own data:

```bash
python twitter_sentiment_main.py
```

This script will:
- Load and preprocess `Twitter_Data.csv`
- Train an LSTM model with an Embedding layer
- Save the trained model as `sentiment_model.h5`
- Save the tokenizer as `tokenizer.joblib`

Make sure your input data file (`Twitter_Data.csv`) has a `clean_text` column and a `sentiment` label.

---

## ✅ Requirements

- Python 3.7+
- TensorFlow
- Streamlit
- scikit-learn
- pandas
- numpy
- joblib

All dependencies are listed in `requirements.txt`.

---

## 📬 Contact

For suggestions or issues, feel free to raise an issue or fork and contribute to this project.

---

## 🔐 License

This project is open-source and free to use under the MIT License.
