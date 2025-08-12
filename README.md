# Task 6: Sales Trend Analysis Using Aggregations

## 📌 Objective
Analyze **monthly revenue** and **order volume** from an `orders` table using SQL aggregate functions and grouping.

---

## 📂 Dataset
Since no dataset was provided, a **sample dataset** was created for demonstration.  
Table: `orders`  
Columns:
- **order_id** (INT) – Unique order identifier
- **order_date** (DATE) – Date of the order
- **amount** (DECIMAL) – Revenue from the order (can be NULL)
- **product_id** (INT) – Product identifier

---

## 🛠️ Tools Used
- **SQLite** via [Programiz Online SQL Compiler](https://www.programiz.com/sql/online-compiler)

---

## 🗄️ Sample Data
```sql
CREATE TABLE orders (
    order_id INT,
    order_date DATE,
    amount DECIMAL(10,2),
    product_id INT
);

INSERT INTO orders (order_id, order_date, amount, product_id) VALUES
(1, '2023-01-05', 250.00, 101),
(2, '2023-01-15', 150.00, 102),
(3, '2023-02-02', 350.50, 103),
(4, '2023-02-10', 120.00, 104),
(5, '2023-03-05', 200.00, 105),
(6, '2023-03-15', NULL,     106), -- Null amount to test handling
(7, '2023-04-12', 500.00, 107),
(8, '2023-04-25', 320.00, 108),
(9, '2023-05-01', 450.00, 109),
(10,'2023-05-18', 300.00, 110),
(11,'2023-06-03', 210.00, 111),
(12,'2023-06-20', 400.00, 112);
