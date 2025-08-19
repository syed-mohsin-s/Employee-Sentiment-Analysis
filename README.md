# Employee Sentiment Analysis 🚀

This project analyzes employee feedback using **Transformer-based NLP models** to identify sentiment, calculate employee scores, rank employees, and detect flight risks. Finally, an interactive **Streamlit dashboard** provides insights for HR managers.

---

## 📌 Project Workflow

### **Task 1 – Sentiment Classification**
- Used `DistilBERT` fine-tuned on employee feedback (`feedback_clean` column).
- Preprocessed data and trained with HuggingFace `Trainer`.
- Generated predictions (`test_set_with_sentiment.csv`) with confidence scores.

### **Task 2 – Exploratory Data Analysis (EDA)**
- Explored feedback distribution, missing values, and sentiment balance.
- Visualizations:
  - Sentiment distribution (train/test)
  - Monthly sentiment trends
  - Top employees by feedback count
  - WordClouds for positive & negative feedback

### **Task 3 – Employee Score Calculation**
- Converted predicted sentiments into numeric scores:
  - Positive = +1  
  - Negative = –1  
  - Neutral = 0  
- Calculated **per-employee sentiment scores** (monthly if `reviewed` available, otherwise overall).

### **Task 4 – Employee Ranking**
- Ranked employees based on sentiment scores.
- Ranking available both **monthly** and **globally**.

### **Task 5 – Flight Risk Identification**
- Identified **High / Medium / Low risk** employees based on:
  - Sentiment score
  - Rank percentile
- Generated `employee_flight_risk.csv` for HR insights.

### **Task 6 – Dashboard**
- Built an interactive **Streamlit dashboard** with:
  - Sentiment distribution  
  - Trends over time  
  - Employee scores  
  - Rankings  
  - Flight risk levels  

Run dashboard:
```bash
streamlit run dashboard.py
