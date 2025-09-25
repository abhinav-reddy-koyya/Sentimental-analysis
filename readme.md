# 🐦 Twitter Sentiment Analysis

## 📌 Overview
This project performs sentiment analysis on **Twitter airline reviews dataset**.  
It includes preprocessing, visualization, model training, and a **Streamlit web app** for real-time sentiment predictions.

---

## 📂 Project Structure
data/
├── raw/ (original Tweets.csv)
├── processed/ (cleaned dataset)
models/
└── sentiment_model.pkl
notebooks/
├── 01_EDA.ipynb
├── 02_Modeling.ipynb
utils/
├── preprocessing.py
├── visualization.py
├── sentiment_model.py
outputs/
└── charts/
app.py
requirements.txt

yaml
Copy code

---

## ⚙️ Setup Instructions
1. Clone repo & create venv
```bash
git clone <repo_url>
cd sentimental-analysis
python -m venv venv
venv\Scripts\activate   # On Windows
Install requirements

bash
Copy code
pip install -r requirements.txt
Preprocess data

bash
Copy code
python utils/preprocessing.py
Train model

bash
Copy code
python utils/sentiment_model.py
Run visualization

bash
Copy code
python utils/visualization.py
Launch Streamlit app

bash
Copy code
streamlit run app.py
📊 Features
Preprocessing (cleaning tweets: stopwords, stemming, hashtags removal)

Exploratory Data Analysis with charts

Logistic Regression model with TF-IDF features

Streamlit dashboard for predictions

🚀 Example
Input:

arduino
Copy code
"This flight was terrible and delayed."
Output:

yaml
Copy code
Predicted Sentiment: negative
🔮 Future Work
Use LSTMs or BERT for better accuracy

Add word clouds for positive/negative reviews

Deploy on AWS / Heroku

yaml
Copy code

---

✅ Now you can:
1. Run preprocessing → saves `tweets_clean.csv`
2. Train model → saves `sentiment_model.pkl`
3. Run app → interactively test tweets  