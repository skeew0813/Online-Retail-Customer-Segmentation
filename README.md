# Customer Segmentation and Sales Analysis (Online Retail 2011)

This project explores customer purchasing behavior using RFM segmentation and monthly sales trends from the Online Retail 2011 dataset. The goal was to understand which customers provide the most value, how behavior varies across segments, and when major revenue spikes occur throughout the year.

> **My role in this project:** Presentation and data storytelling — I designed the slide deck, organized the team’s analytical findings, and delivered the final presentation.

---

## 📊 Project Overview

This analysis was designed to help a retail business answer key questions such as:

- Which customers contribute the most revenue?
- How are customers distributed across Recency, Frequency, and Monetary (RFM) segments?
- What seasonal trends exist in monthly sales?
- Which product categories drive demand throughout the year?
- What short-term sales forecasts can be made moving into early 2012?

The project combines RFM scoring with time series analysis to uncover actionable customer and revenue insights.

---

## ⚙️ Methods Used by the Team

| Step | Description |
|------|-------------|
| **Data Cleaning** | Removed canceled invoices, handled missing CustomerID fields, filtered invalid transactions. |
| **Feature Engineering** | Created Recency, Frequency, and Monetary metrics for every customer. |
| **RFM Segmentation** | Assigned each customer a 3-digit score (e.g., `444`, `344`, `212`) to group behavior patterns. |
| **Visualization** | Charted customer distributions, segment performance, monthly sales, and product category trends. |
| **Time Series Analysis** | Aggregated monthly sales and built an ARIMA model to forecast revenue for early 2012. |

---

## 🧠 Key Insights Identified by the Team

- Most customers purchased **very few times**, with a long tail representing more engaged buyers.  
- High-value RFM segments (like **444**) produced dramatically higher average monetary value compared to other segments.  
- Sales showed a clear seasonal spike in **Q4**, driven by holiday shopping behavior.  
- “Other” products generated the most revenue overall, but **Seasonal** and **Gifts** categories surged in Q4.  
- Countries like **Netherlands** and **Australia** had lower total sales but **higher average order values**, suggesting region-specific opportunities.

---

## 📈 Core Visuals

<p align="center">
  <img src="visuals/rfm_segment_distribution.png" alt="Distribution of RFM segments across customers" width="800">
</p>

<p align="center">
  <img src="visuals/rfm_avg_monetary.png" alt="Average monetary value by RFM segment" width="800">
</p>

<p align="center">
  <img src="visuals/monthly_sales_trend_2011.png" alt="Monthly sales trend with holiday spike highlighted" width="800">
</p>

<p align="center">
  <img src="visuals/monthly_sales_by_category.png" alt="Monthly sales by product category (stacked area)" width="800">
</p>

Additional visuals, including recency/frequency distributions, ARIMA forecasting results, and country-level comparisons, are available in the `visuals/` folder.

---

## 🧰 Tech Stack

- **Python**
- pandas, NumPy  
- Matplotlib, seaborn  
- statsmodels (ARIMA)

---

## 🧩 How to Run

1. Clone the repo:

    ```bash
    git clone https://github.com/skeew0813/Online-Retail-Customer-Segmentation.git
    cd Online-Retail-Customer-Segmentation
    ```

2. (Optional) Create and activate a virtual environment:

    ```bash
    python -m venv .venv
    # Windows:
    .venv\Scripts\activate
    # macOS/Linux:
    source .venv/bin/activate
    ```

3. Install dependencies:

    ```bash
    pip install pandas numpy matplotlib seaborn statsmodels jupyter
    ```

4. Launch Jupyter:

    ```bash
    jupyter notebook
    ```

5. Open:

    ```
    notebooks/Customer_Analysis_Notebook.ipynb
    ```

---

## 📚 References

- Online Retail Dataset (Kaggle):  
  https://www.kaggle.com/datasets/vijayuv/onlineretail

- Original UCI Dataset Source:  
  Hofmann, H. (2011). Online Retail Data Set (UCI Machine Learning Repository).

---

## 🧾 Attribution

This project was completed collaboratively with classmates at Bellevue University.  
I served as the **Presenter**, responsible for transforming the team’s analysis into a structured presentation, designing the slides, and communicating key insights to stakeholders.

