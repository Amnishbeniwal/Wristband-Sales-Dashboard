# 🧮 DAX Measures – Wristband Sales Dashboard

## 🔹 Sales Measures

### Total Sales
SUM(Orders[total_value])

### Item Level Sales
SUMX(
    Order_Items,
    Order_Items[item_price] * Order_Items[qty]
)

### Net Sales
Item Level Sales - SUM(Order_Items[discount_amount])

### Average Order Value (AOV)
DIVIDE([Total Sales], [Total Orders])

---

## 🔹 Order Measures

### Total Orders
DISTINCTCOUNT(Orders[order_id])

---

## 🔹 Customer Measures

### Total Customers
DISTINCTCOUNT(Customers[customer_id])

### Repeat Customers
CALCULATE(
    DISTINCTCOUNT(Orders[customer_id]),
    FILTER(
        VALUES(Orders[customer_id]),
        CALCULATE(COUNT(Orders[order_id])) > 1
    )
)

### Repeat Customer %
DIVIDE([Repeat Customers], [Total Customers])

---

## 🔹 Discount Measures

### Total Discount
SUM(Order_Items[discount_amount])

### Discount Impact %
DIVIDE([Total Discount], [Item Level Sales])

---

## 🔹 Payment Measures

### Total Paid Amount
SUM(Payments[amount])

### Successful Payments
CALCULATE(
    COUNT(Payments[payment_id]),
    Payments[payment_status] = "Success"
)

### Payment Success Rate
DIVIDE([Successful Payments], COUNT(Payments[payment_id]))

---

## 🔹 Review Measures

### Average Rating
AVERAGE(Reviews[rating])

### Total Reviews
COUNT(Reviews[review_id])
