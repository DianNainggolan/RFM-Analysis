# RFM Analysis on Online Retail and Amazon Customer Segmentation

This project applies **RFM (Recency, Frequency, Monetary)** analysis to understand customer behavior and segment customers from online retail data, including insights relevant to **Amazon’s e-commerce ecosystem**. The analysis aims to identify loyal customers, at-risk segments, and opportunities for retention and marketing optimization.

---

## 🧠 Business Understanding

Modern e-commerce platforms such as **Amazon** rely heavily on **customer segmentation** to tailor marketing, recommend products, and improve retention. RFM Analysis is a widely used technique for this purpose, focusing on three behavioral metrics:

* **Recency (R):** How recently a customer made a purchase.
* **Frequency (F):** How often the customer makes purchases.
* **Monetary (M):** How much the customer spends in total.

By combining these three scores, Amazon and similar platforms can classify customers into actionable segments — such as *Champions*, *Loyal Customers*, *At Risk*, *Hibernating*, and *Potential Loyalists*.

---

## 📊 Data Understanding

**Data Source:** Kaggle – Online Retail Dataset
**Columns Used:**

* `CustomerID` – Unique customer identifier
* `InvoiceDate` – Transaction timestamp
* `Quantity` – Number of items purchased
* `Price` – Price per item

The dataset represents global online retail transactions, similar in structure to what Amazon would process from its marketplace data.

---

## 🧩 RFM Segmentation Process

1. **Recency:** Calculated as the number of days since the last purchase.
2. **Frequency:** Number of completed orders per customer.
3. **Monetary:** Total revenue per customer (`Quantity × Price`).

Each customer is scored (1–5) for R, F, and M, then combined into an **RFM score** such as `555` (Champions) or `111` (Lost Customers).

---

## 📈 RFM Score Matrix Insights

* **Recency:** Few customers are active within the past 5 months; most are dormant.
* **Frequency:** Majority of users have fewer than 5 purchases — indicating low loyalty.
* **Monetary:** Most customers spend under $5,000, showing a long-tail pattern typical of Amazon’s customer base.

---

## 📉 Segmentation Results

* **At Risk** — Largest customer group; previously active but now inactive.
* **Potential Loyalist** — Second largest; promising group for retention campaigns.
* **Hibernating** — Dormant users with low activity and spending.
* **Champions** — Smallest group but with the highest total spend and frequency.
* **Need Attention / Promising / New Customers** — Smaller segments, ideal for nurturing via personalized marketing.

---

## 🛒 Amazon Context

Amazon exemplifies large-scale RFM application:

* Uses **Recency** and **Frequency** to power dynamic recommendation systems (e.g., “Buy Again” and “Related to your last purchase”).
* Applies **Monetary** scoring to identify high-value customers for programs like **Prime** and **Personalized Ads**.
* Integrates RFM data into machine learning pipelines to predict **Customer Lifetime Value (CLV)** and churn risk.

The same RFM principles demonstrated in this project can scale to millions of users and transactions on Amazon’s retail and marketplace ecosystems.

---

## 📚 Conclusion

RFM analysis effectively segments online retail customers, providing a foundation for personalized marketing, retention, and predictive modeling.
While this project focuses on a single retail dataset, its approach mirrors Amazon’s customer intelligence strategies — leveraging behavioral metrics to maximize value and engagement across its vast digital marketplace.
