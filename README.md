# 📊 Multi-Source Market Intelligence System

An end-to-end data analytics project that integrates **cryptocurrency market data** and **global news sentiment** to analyze how sentiment regimes influence **market volatility and returns**.  
The project uses **Bitcoin** as a case study and focuses on **explainable, descriptive insights** rather than prediction.

---

## 🔍 Project Overview

Financial markets are influenced not only by price dynamics but also by news and public sentiment.  
This project builds a complete pipeline that:

- Collects **Bitcoin price data** from a market API  
- Extracts **news headlines** related to cryptocurrency  
- Converts text data into **sentiment scores using NLP**
- Engineers **returns, volatility, and sentiment regimes**
- Analyzes how market behavior differs across sentiment states  

The goal is to understand **risk behavior under different sentiment conditions**.

---

## 🧠 Key Insights

- **Negative sentiment regimes** are associated with **higher market volatility**
- **Returns vary only modestly** across sentiment states
- Sentiment impacts **market risk more than return direction**
- Volatility shows **clustering**, indicating periods of sustained uncertainty
- News sentiment is **event-driven**, not continuous

---

## 🏗️ Workflow & Methodology

1. **Market Data Collection**
   - Bitcoin historical prices via CoinGecko API
   - Daily frequency (last 180 days)

2. **News Data Collection**
   - Global news headlines via GDELT API
   - Cryptocurrency-related keyword filtering

3. **Sentiment Analysis**
   - Rule-based NLP using VADER
   - Extracted positive, negative, neutral, and compound scores

4. **Feature Engineering**
   - Daily returns
   - Rolling volatility (7, 14, 30 days)
   - Sentiment regime classification

5. **Exploratory Data Analysis**
   - Price trends
   - Return distributions
   - Volatility clustering
   - Price vs sentiment comparison

6. **Regime-Based Analysis**
   - Comparison of returns and volatility across:
     - Positive sentiment
     - Neutral sentiment
     - Negative sentiment

---

## 📊 Sentiment Regime Definition

| Sentiment Regime | Compound Score Range |
|-----------------|----------------------|
| Positive        | ≥ 0.05               |
| Neutral         | (-0.05, 0.05)        |
| Negative        | ≤ -0.05              |

---

## 🧪 Technologies Used

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **VADER Sentiment Analysis**
- **REST APIs**
  - CoinGecko
  - GDELT

---

---

## ⚙️ Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/your-username/market-sentiment-intelligence.git
cd market-sentiment-intelligence

2. Install dependencies:
pip install -r requirements.txt

3. Run the notebook:
jupyter notebook notebooks/Market_Sentiment_Analysis.ipynb

---
## ⚠️ Limitations

- The analysis is **descriptive**, not causal; sentiment does not directly explain price movements.
- News coverage is **uneven across dates**, leading to missing sentiment on some days.
- Cryptocurrency markets are influenced by multiple external factors not captured in this project.
- Rule-based sentiment analysis (VADER) may miss context, sarcasm, or domain-specific language.
- The study focuses on a **single asset (Bitcoin)**, limiting generalizability.

---

## 🙌 Author

**Anushka Khadatkar**  
Data Analyst | Data Science Enthusiast

