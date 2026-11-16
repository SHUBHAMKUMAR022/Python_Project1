# Project Summary – E-Commerce Sales Analyzer (PS 26)

1. ## Problem Statement
Analyze online order data from a CSV file to find total revenue, units sold, best-selling products and category-wise revenue using aggregation, and visualise the results[cite: 1].
It must handle data cleaning, duplicate removal, invalid quantity/price handling, and display Matplotlib bar and pie charts[cite: 1].

## 2. Approach
- **Data Handling:** Reads online order data from a CSV file (`orders.csv`) using Pandas[cite: 1].
- **Data Cleaning & Validation:** Validates each row, skipping duplicates, non-positive values, or invalid strings for quantities and prices with detailed console error logs.
- **Aggregation:** Computes revenue per order ($\text{Quantity} \times \text{Price}$)[cite: 1], total revenue, total orders, units sold, and product-wise revenue.
- **Visualization & Menu:** Provides an interactive console menu to view overall summaries, category-wise percentage shares with a Pie chart, and top-selling products using a Bar chart via Matplotlib[cite: 1].

## 3. Test Cases (run from `orders.csv`)

| # | Input | Expected Output | Result |
|---|-------|-----------------|--------|
| 1 | Normal Input (`orders.csv` with 3 valid orders, Menu Option 1) | Total Revenue: 32500 \| Orders: 3<br>Units sold: 8 \| Top product: Phone (30000)[cite: 1] | Pass |
| 2 | Boundary / Minimum Input (`orders.csv` with 1 row, Menu Option 1) | Total Revenue: 10 \| Orders: 1<br>Units sold: 1 \| Top product: Pen[cite: 1] | Pass |
| 3 | Invalid Input (`orders.csv` with invalid quantity/price, Menu Option 1) | Row 2 skipped: invalid Quantity 'abc'<br>Row 3 skipped: Price must be positive<br>Total Revenue: 20000 \| Orders: 1[cite: 1] | Pass |
| 4 | Different Valid Scenario (Same CSV as Test Case 1, Menu Option 2) | Electronics: 30000 (92.31%)<br>Fashion: 2500 (7.69%)<br>Pie chart 'Category-wise Revenue' displayed[cite: 1] | Pass |

## 4. Screenshots

> Run the program, take a screenshot of each menu option/test case and save it in the `screenshots/` folder.

**Test Case 1 – Normal Input**
![Test Case 1](screenshots/test1.png)

**Test Case 2 – Boundary Input**
![Test Case 2](screenshots/test2.png)

**Test Case 3 – Invalid Input**
![Test Case 3](screenshots/test3.png)

**Test Case 4 – Different Valid Scenario**
![Test Case 4](screenshots/test4.png)

## 5. Conclusion
The program meets all requirements of PS 26 and passes all four test cases[cite: 1]. Possible improvements: a graphical user interface (GUI), exporting reports to Excel/PDF, and integrating a database instead of a CSV file.
```[cite: 1]
