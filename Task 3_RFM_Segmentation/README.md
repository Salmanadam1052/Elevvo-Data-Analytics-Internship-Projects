

---

# RFM Customer Segmentation Analysis

## Overview

This project performs **RFM (Recency, Frequency, Monetary) analysis** on an e-commerce dataset (`OnlineRetail.xlsx`) to segment customers based on their purchasing behavior. It provides insights into customer value, retention, and loyalty through interactive visualizations using **Plotly**.

---

## Dataset

* **File:** `OnlineRetail.xlsx`
* **Source:** Online retail transactions
* **Key Columns:**

  * `InvoiceNo` – Unique invoice number
  * `StockCode` – Product code
  * `Description` – Product description
  * `Quantity` – Number of items purchased
  * `InvoiceDate` – Date of transaction
  * `UnitPrice` – Price per unit
  * `CustomerID` – Unique customer identifier
  * `Country` – Customer location

---

## Data Cleaning

1. Removed missing values in `CustomerID` and `Description`.
2. Removed negative values in `Quantity` and `UnitPrice` (likely returns).
3. Excluded canceled invoices starting with 'C'.
4. Added a `TotalPrice` column: `Quantity * UnitPrice`.
5. Converted `InvoiceDate` to datetime format.

---

## RFM Analysis

* **Recency (R):** Days since the last purchase
* **Frequency (F):** Number of orders placed
* **Monetary (M):** Total money spent

**RFM Scores:**

* `R_Score`, `F_Score`, `M_Score` – Quartile-based scoring
* `RFM_Segment` – Combined string of R, F, M scores
* `RFM_Score` – Sum of R, F, M scores

**Customer Segments:**

* Champions (RFM Score ≥ 10)
* Loyal Customers (Score ≥ 8)
* Potential Loyalist (Score ≥ 6)
* Need Attention (Score ≥ 4)
* At Risk (Score < 4)

---

## Visualizations

1. **Customer Segment Distribution** – Bar chart of customer segments
2. **Monetary Distribution** – Boxplot with log scale by segment
3. **Average RFM Metrics by Segment** – Grouped bar chart
4. **Customer Count Heatmap (R vs F)** – Heatmap of Recency vs Frequency
5. … (Additional charts can include Frequency distribution, Recency distribution, Monetary distribution by segment, etc.)

All visualizations are interactive using **Plotly** with dark theme styling.

---

## Dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly openpyxl
```

---

## How to Run

1. Load the dataset (`OnlineRetail.xlsx`).
2. Run the Python script to perform data cleaning, RFM scoring, and customer segmentation.
3. Interactive charts will be displayed automatically using Plotly.

---

## Contact

**Author:** Salman Adam
**LinkedIn:** [www.linkedin.com/in/salmanadam](https://www.linkedin.com/in/salmanadam)


