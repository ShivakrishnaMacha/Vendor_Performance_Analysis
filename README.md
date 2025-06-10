# 📦 Vendor Performance Analysis

## 📘 Overview

This project focuses on evaluating vendor performance and inventory efficiency in a retail/wholesale business context. By analyzing key metrics related to pricing, sales, inventory turnover, and vendor contribution, we aim to support smarter decision-making that drives profitability and minimizes operational risks.

---

## ❓ Business Context

Retail and wholesale businesses often struggle with challenges such as:

- Products that don't sell but still incur storage costs.
- Vendors with inconsistent supply or limited contribution to profits.
- High shipping costs or inefficient pricing models.
- Stock that moves slowly, tying up capital unnecessarily.

### 🔍 Key Questions

1. **Which brands underperform and need price or promotional changes?**
2. **Which vendors generate the most sales and profit?**
3. **Does buying in bulk reduce costs effectively?**
4. **Which vendors have low inventory turnover and need review?**
5. **How do profit margins differ between top and low-performing vendors?**

---

## 📊 Dataset Summary

The dataset includes transaction-level and inventory information with columns such as:

- **Brand, Vendor, Product Code**
- **Total Sales Quantity, Sales Revenue**
- **Gross Profit, Profit Margin**
- **Purchase Price, Actual Selling Price**
- **Freight Cost, Stock Turnover Ratio**

### ⚠️ Data Observations

- Some records show **negative or zero gross profit** due to selling below cost.
- **Zero sales quantities** imply inventory that was purchased but never sold.
- A few **outliers** with high prices and freight charges suggest premium products or bulk shipping costs.

To maintain reliability, we filtered out:
- Transactions with zero or negative profit or margin.
- Inventory with zero sales volume.

---

## 📈 Exploratory Data Analysis (EDA)

### 📉 Summary Stats

- **Gross Profit** ranged from -52,002.78 to significant highs.
- **Profit Margin** included extreme values due to zero revenue in some cases.
- **Purchase & Actual Prices** showed high variance — up to $7,499.99.
- **Freight Costs** varied greatly, indicating irregular logistics costs.

### 🔗 Correlation Insights

- **Purchase Price vs. Sales & Profit**: Very weak correlation, suggesting price changes don’t directly impact profits.
- **Sales Quantity vs. Purchase Quantity**: Very strong correlation (0.999), confirming effective inventory flow.
- **Profit Margin vs. Sales Price**: Negative correlation (-0.179), possibly due to pricing competition.
- **Stock Turnover vs. Profitability**: Minimal correlation; fast-moving products don’t always mean higher profits.

---

## 🧠 Key Findings

### 1. 🚩 Brands Requiring Pricing or Promotion

- 198 brands show low sales volume but high margins — a good opportunity for targeted promotions or discounts to increase volume without hurting profitability.

### 2. 🏆 Vendor Sales Contribution

- Top 10 vendors account for **65.69%** of all purchases.
- Heavy reliance on these few vendors increases **supply chain risk**.

### 3. 📦 Bulk Purchase Impact

- Vendors offering **bulk discounts** reduce unit cost by **up to 72%**.
- Strategic bulk buying boosts overall profitability.

### 4. 🛑 Low Inventory Turnover

- Unsold stock accounts for **$2.71 million** in capital.
- Slow-moving stock increases holding costs and affects cash flow.

### 5. 💰 Vendor Profit Margin Comparison

- **Top vendors' margin:** ~31.17%
- **Low-performing vendors' margin:** ~41.55%
- Higher margins among low-performing vendors may point to **pricing inefficiencies** or limited market access.

---

## 📐 Statistical Validation

### Hypothesis Test:

- **Null Hypothesis (H₀):** No significant difference in profit margins.
- **Alternate Hypothesis (H₁):** A significant difference exists.

✅ Result: **Reject H₀**  
This confirms that high-margin vendors and top-selling vendors operate under different profitability models.

---

## 📊 Power BI Dashboard

Here’s a snapshot of the Power BI dashboard used to visualize key insights:

![Image](https://github.com/user-attachments/assets/55a4f605-037f-469e-908f-05a694d25622)

🔗 [Click here to view the interactive Power BI dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTlkNzUwYzMtYzY3OC00ZGU5LWJhZjMtN2JmYmJkZWE3ZGJmIiwidCI6IjZhYjJmZGI1LWNjOWUtNDJiMy04ZmI5LTA4ZWU1OGI5YzRhMSJ9)

> Replace the above image path and link with your actual image and published Power BI dashboard link.

---

## 🛠️ Tools Used

- **Python** (Pandas, Matplotlib, Seaborn, NumPy, Scikit-learn)
- **Jupyter Notebook** for data cleaning and EDA
- **Power BI** for interactive business intelligence dashboards

---

## 📁 Files Included

- `Exploratory_Data_Analysis.ipynb`: Complete analysis notebook
- `PowerBI_Report.pbix`: Dashboard file (Power BI)
- `README.md`: Documentation

---

## ✅ Recommendations

- Adjust prices or run promotions on low-sale, high-margin products.
- Reduce vendor dependency by partnering with a broader supplier base.
- Leverage bulk purchasing to maintain cost-effective inventory.
- Review low-turnover products to avoid stockpiling and reduce storage costs.
- Strengthen marketing and logistics support for vendors with strong margins but poor sales.

---

## 📌 Conclusion

This vendor performance analysis highlights areas for operational and strategic improvements. It brings together data science, business intelligence, and domain knowledge to drive efficient inventory control, better vendor management, and sustainable profit growth.

---

## 📬 Contact

**Shivakrishna Macha**  
[LinkedIn](https://www.linkedin.com/in/shivakrishnamacha/) | [GitHub](https://github.com/ShivakrishnaMacha/Data-Analysis-and-Visualization-Project-Portfolio)
