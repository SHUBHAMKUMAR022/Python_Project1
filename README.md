# Python_Project1
# E-Commerce Sales Analyzer (PS 26)

An interactive console-based Python 3 program to analyze online order data, calculate revenue, units sold, best-selling products, and category-wise sales with visual charts.  
Built for **Rungta International Skills University – School of Computer Science and Engineering (B.Tech CSE)**.

## Repository Structure
E-Commerce-Sales-Analyzer/
├── sales_analyzer.py # Complete solution (single Python file)
├── Readme.md         # Describes the repository (this file)
├── orders.csv        # Input dataset containing online order records
└── screenshots/      # Output screenshots and generated charts
`orders.csv` is used as the source data file and can be customized or will be created automatically if empty/missing.

## Features

- Read and parse online order data from a CSV file using Pandas
- Clean data by skipping invalid quantities, non-positive prices, and duplicate order IDs with detailed error logs
- Calculate revenue per order ($\text{Revenue} = \text{Quantity} \times \text{Price}$)
- Compute total revenue, total orders, units sold, and identify top-selling products[cite: 1]
- Generate category-wise revenue percentages and visual charts (Bar and Pie charts using Matplotlib)[cite: 1]
- Interactive menu system to select different analysis options

## Concepts Used

Python 3, Pandas (CSV handling & data aggregation)[cite: 1], Matplotlib (Data visualization)[cite: 1], Exception Handling, and Modular Programming.

## Available Menu Options

| Option | Action Description |
|--------|--------------------|
| 1 | View Overall Summary (Total Revenue, Orders, Units Sold, Top Product)[cite: 1] |
| 2 | View Category-wise Revenue & Display Pie Chart[cite: 1] |
| 3 | View Top 5 Selling Products & Display Bar Chart[cite: 1] |
| 4 | Exit the Application |

## How to Run

   1. Ensure Python 3 along with required libraries are installed:
      ```bash
      pip install pandas matplotlib
1.Place your orders.csv file in the same directory.

2.Run the script from your console/terminal[cite: 1]:
Bash
   python sales_analyzer.py
   
Data File Format
Each line in orders.csv: Order_ID,Product,Category,Quantity,Price

Example: O1,Phone,Electronics,2,10000[cite: 1]

Requirements
Python 3.x, Pandas, Matplotlib[cite: 1].
