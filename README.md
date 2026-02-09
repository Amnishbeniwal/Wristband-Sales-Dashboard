# 📊 Sales & Customer Analytics – Wristband E-Commerce

## 📌 Project Overview
This project presents a 3-page Power BI dashboard designed for a custom wristband e-commerce business similar to Wrist-Band.com.  
The dashboard provides insights into sales performance, product demand, customer behavior, payment efficiency, and product quality.

---

## 🎯 Business Objectives
- Monitor overall sales and revenue trends
- Identify top-performing wristband categories and products
- Analyze customer demographics and repeat behavior
- Track payment success and failures
- Evaluate product quality using customer reviews

---

## 🗂️ Dataset Description
The dataset consists of 6 tables:
- **Customers** – customer demographics and location
- **Products** – wristband categories, sub-categories, and pricing
- **Orders** – order-level transaction data
- **Order_Items** – product-level sales and discounts
- **Payments** – payment methods and payment status
- **Reviews** – customer ratings and review dates

---

## 🧱 Data Model
- Star schema design
- One-to-many relationships
- Sales calculated at item level to ensure correct category and product analysis

---

## 📊 Dashboard Pages

### 🟦 Page 1: Executive Sales Overview
- Total Sales, Net Sales, Orders, AOV, Customers
- Sales trend over time
- Sales by category and country
- Order status distribution

### 🟦 Page 2: Product & Customer Insights
- Top-selling wristband products
- Category and sub-category analysis
- Discount vs Net Sales comparison
- Customer age group and regional analysis

### 🟦 Page 3: Payments & Product Quality
- Payment success rate and method analysis
- Orders vs successful payments
- Product rating distribution
- Identification of low-rated products

---

## 🧮 Key Metrics & DAX
- Net Sales
- Average Order Value
- Repeat Customer %
- Discount Impact
- Payment Success Rate
- Average Product Rating

(See `DAX_Measures.md` for full list)

---

## 💡 Key Insights
- Silicone wristbands generate the highest revenue
- Customers aged 18–35 contribute the most sales
- High discounts impact net margins in some categories
- Card payments show the highest success rate
- Products with ratings below 3 require quality improvement

---

## 🛠 Tools Used
- Power BI
- DAX
- Data Modeling (Star Schema)

---

## 📌 Outcome
This dashboard enables stakeholders to make data-driven decisions related to pricing, marketing strategy, payment optimization, and product quality improvements.
