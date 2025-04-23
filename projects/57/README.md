# 🎵 Maven Music Cancellation Predictor

# 🎵 Streamlit Application: https://huggingface.co/spaces/lenaras/cancellation_prediction


## 🚀 Project Summary

This project uses listening behavior and subscription data to **predict customer cancellations** for a music streaming platform (Maven Music). It applies logistic regression and other machine learning techniques to build a model capable of identifying at-risk customers.

### 🧠 Key Features
- Cleaned and joined 4 related datasets (customers, sessions, listening history, audio).
- Engineered features like:
  - Number of sessions
  - % Pop music listening
  - % Podcast listening
  - Whether the customer had a discount
- Built a predictive model (Logistic Regression)
- Deployed as a **Streamlit App** on Hugging Face

---

## 📊 Insights

| Insight | Description |
|--------|-------------|
| 💰 Discounted customers | ~86% of them cancelled — strongest predictor! |
| 🎧 Listening Sessions | Fewer sessions = higher cancellation risk |
| 🎶 Pop Music % | Higher % Pop listening = increased cancellations |
| 🎙️ Podcast Listening | No clear correlation to cancellation |

---

## 🧪 Model Performance

| Metric | Value |
|--------|--------|
| Accuracy | 100% (on test split) |
| ROC AUC (5-Fold CV) | 0.82 |
| Avg Precision | 0.74 |
| Model Used | Logistic Regression |

---

## 🔍 How to Use

1. Clone the repo or deploy via Hugging Face
2. Launch the Streamlit app:

```bash
streamlit run app.py
