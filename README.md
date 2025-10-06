# 🍽 Sentiment Analysis of Swiggy vs Zomato App Reviews
### Text Analytics and NLP Project in Python  

---

## 🎯 Project Overview
This project applies **Text Analytics and Natural Language Processing (NLP)** techniques to analyze customer reviews from the **Google Play Store** for two major Indian food delivery apps — **Swiggy** and **Zomato**.

The goal is to:
- Analyze customer sentiment (Positive / Neutral / Negative)
- Identify recurring keywords and bigrams in reviews
- Compare public perception of both brands
- Generate actionable insights for product and service improvement

---

## ⚙️ Tech Stack
| Category | Tools / Libraries |
|-----------|------------------|
| Data Collection | `google-play-scraper` |
| Text Cleaning | `NLTK`, `spaCy`, `re`, `emoji` |
| Sentiment Analysis | `VADER`, `TextBlob`, `Scikit-learn` |
| Visualization | `Matplotlib`, `Seaborn`, `WordCloud`, `Plotly` |
| Storage | `Pandas`, `Google Drive` |
| Environment | Google Colab (Python 3) |

---

## 🧩 Workflow

### 1️⃣ Data Collection  
Scraped ~10,000 latest user reviews from the Google Play Store using the `google-play-scraper` library for:
- Swiggy (`in.swiggy.android`)  
- Zomato (`com.application.zomato`)

### 2️⃣ Data Cleaning  
- Removed punctuation, emojis, URLs, and stopwords  
- Performed tokenization and lemmatization using `spaCy`  
- Converted all text to lowercase  

### 3️⃣ Sentiment Analysis  
- Applied **VADER** for rule-based sentiment scoring  
- Used **TextBlob** for polarity scoring (-1 to +1)  
- Created a **blended sentiment metric** combining both  

### 4️⃣ Visualization  
Generated:
- Sentiment distribution bar charts  
- TextBlob polarity boxplots  
- Word clouds for positive and negative reviews  
- Top bigrams to capture frequent issue themes  

### 5️⃣ Insights Extraction  
- Quantified sentiment share per app  
- Compared sentiment alignment with star ratings  
- Identified most-liked negative reviews for product improvement  

---

## 📊 Key Findings

| Observation | Insight |
|--------------|----------|
| **Zomato** – ~74% positive reviews | Higher customer satisfaction and brand sentiment |
| **Swiggy** – ~60% positive reviews | Mixed sentiment; common issues around delivery delays and refunds |
| **Common Pain Points** | "late delivery", "refund not processed", "order cancel" |
| **Validation** | Sentiment polarity closely matches user star ratings |

---

## 💡 Business Recommendations
| Area | Recommendation |
|------|----------------|
| Delivery Reliability | Improve ETA accuracy and real-time tracking |
| Refund Process | Simplify refund policies and automate notifications |
| Customer Support | Introduce faster AI/live chat assistance |
| Feedback Monitoring | Use real-time dashboards for review tracking |

---

## 🧠 Future Enhancements
- Apply **Topic Modeling (LDA)** to identify hidden themes  
- Extend to **multi-language reviews** (Hindi, Tamil, Telugu, etc.)  
- Build a **Streamlit dashboard** for real-time sentiment updates  
- Integrate aspect-based sentiment analysis (e.g., delivery, price, UI)
