# 💳 Digital Payments Analysis (PhonePe Data Project)

## 🚀 Problem Statement

With the rapid growth of digital payments, businesses need to understand transaction trends, regional adoption, and user behavior.
This project analyzes PhonePe transaction data to uncover insights that support strategic decision-making.

---

## 🛠️ Tech Stack

* MySQL
* Power BI
* Excel

---

## 📂 Dataset

* Source: PhonePe transaction dataset
* Data includes:

  * Transaction amount
  * Transaction count
  * State-wise distribution
  * Year and quarter

---

## ⚙️ Approach

1. Cleaned and structured raw data for analysis
2. Designed relational tables in MySQL
3. Performed SQL analysis using:

   * GROUP BY for aggregations
   * ORDER BY for ranking
   * Filtering for regional insights
4. Built interactive Power BI dashboards to visualize:

   * Transaction trends over time
   * State-wise performance
   * Growth patterns

---

## 📊 Key Insights

* Digital transactions show consistent growth over time
* Top states contribute significantly to total transaction volume
* Quarterly trends indicate seasonal variations in usage
* Increasing adoption of digital payments across regions

---

## 📈 Power BI Dashboard

* Visualized transaction trends by year and quarter
* State-wise comparison of transaction volume and value
* KPI cards for total transactions and growth metrics
* Interactive filters for dynamic analysis

---


## 🧠 SQL Sample Queries

```sql
-- Total transactions by state
SELECT state, SUM(transaction_count) AS total_transactions
FROM phonepe_data
GROUP BY state
ORDER BY total_transactions DESC;

-- Yearly transaction trend
SELECT year, SUM(transaction_amount) AS total_amount
FROM phonepe_data
GROUP BY year
ORDER BY year;

-- Top 10 states by transaction amount
SELECT state, SUM(transaction_amount) AS total_amount
FROM phonepe_data
GROUP BY state
ORDER BY total_amount DESC
LIMIT 10;
```

---

## ▶️ How to Use

* Open the Power BI (.pbix) file
* Interact with filters to explore trends and insights

---

## 📌 Conclusion

This project demonstrates how SQL and Power BI can be used together to analyze large-scale transaction data and generate actionable business insights.
It highlights the role of data analytics in understanding digital payment trends and supporting decision-making.
