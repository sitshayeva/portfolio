# 🎯 Marketing A/B Campaign Scorer

An interactive Streamlit dashboard for analyzing and optimizing marketing A/B campaigns through personalized targeting strategies.  
Hosted live at: 👉 [Try the App on Hugging Face Spaces](https://huggingface.co/spaces/lenaras/Marketing-AB-Campaign-Scorer)

---

## 📊 Project Overview

This project applies machine learning techniques to evaluate and enhance marketing campaigns by:

- Segmenting users based on **ad exposure volume**
- Predicting individual **conversion probabilities**
- Recommending actions: **Target** vs **Hold**
- Visualizing threshold-based precision-recall tradeoffs

Built with `XGBoost`, `pandas`, and `Streamlit`, the dashboard uses exposure-aware thresholding for campaign optimization.

---

## 🧠 Model Highlights

- Trained on a real-world **A/B marketing dataset**
- Handles **class imbalance** using `scale_pos_weight`
- Applies **feature engineering**:
  - Time of day (e.g. evening viewers)
  - Day of week (e.g. weekend exposure)
  - Exposure bins (low / medium / high)
- Uses **segment-specific thresholds** to adjust actions

---

## 🔬 Performance Summary

| Segment | Threshold | Precision | Recall | Conversion Rate |
|---------|-----------|-----------|--------|------------------|
| Low     | Auto-calculated | High | Low    | Low              |
| Medium  | Auto-calculated | Balanced | Balanced | Medium       |
| High    | Auto-calculated | Lower Recall | High Precision | Highest |

*Model dynamically tunes thresholds using F1-score optimization for each exposure group.*

---

## 🚀 How to Use the App

1. Upload or simulate user data using sliders and dropdowns.
2. The model calculates the **predicted conversion probability**.
3. Based on exposure level, the dashboard recommends **Target** or **Hold**.

---

## 📦 Local Installation

```bash
git clone https://huggingface.co/spaces/lenaras/Marketing-AB-Campaign-Scorer
cd Marketing-AB-Campaign-Scorer
pip install -r requirements.txt
streamlit run app.py
```

---

## 🖼️ Screenshot

![Dashboard Screenshot](https://huggingface.co/spaces/lenaras/Marketing-AB-Campaign-Scorer/resolve/main/app_screenshot.png)

---

## 📄 Files in This Space

- `app.py`: Streamlit interface
- `requirements.txt`: Package list
- `README.md`: Project overview
- `marketing_AB.csv`: Your dataset (must be uploaded manually)

---

## 🙌 Credits

Created by [Lenara Sitshayeva](https://huggingface.co/lenaras)  
Live App: https://huggingface.co/spaces/lenaras/Marketing-AB-Campaign-Scorer  
