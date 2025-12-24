## 📊 Sales Dashboard – Power BI

### 🔹 Project Overview
The **Sales Dashboard** is an interactive Power BI report designed to analyze sales performance across multiple dimensions such as **profit, quantity, customers, payment modes, and time**.

It helps business users quickly identify trends, top-performing categories, and potential problem areas.

---

### 🔹 Dashboard Preview
![Sales Dashboard Overview](screenshots/overview.png)

---

### 🔹 Key KPIs
- **Total Sales Amount:** 438K  
- **Total Quantity Sold:** 5,615  
- **Total Profit:** 37K  

---

### 🔹 Business Questions Answered
- Which sub-categories generate the highest profit?
- What are the most used payment modes?
- Who are the top customers by sales amount?
- How does profit trend over months and quarters?
- Which months have negative profitability?

---

### 🔹 Visuals Used
- KPI Cards (Amount, Quantity, Profit)
- Bar Chart – Profit by Sub-Category
- Donut Chart – Quantity by Payment Mode
- Bar Chart – Amount by Customer
- Line Chart – Profit by Month
- Quarter Slicer (Q1–Q4)

---

### 🔹 Data Model
**Fact Table**
- Sales  
  - Amount  
  - Quantity  
  - Profit  
  - Date  
  - PaymentMode  

**Dimensions**
- Customer  
- Category / Sub-Category  
- Calendar (Month, Quarter)  

> Star schema modeling was applied to improve performance and readability.

---

### 🔹 DAX Measures (Examples)
```DAX
Total Sales Amount = SUM(Sales[Amount])

Total Quantity = SUM(Sales[Quantity])

Total Profit = SUM(Sales[Profit])

