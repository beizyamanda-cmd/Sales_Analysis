# Day 2 Sales Analytics

## Project Overview
This project analyzes electronics sales data for Tech Hub Kenya using Python. The notebook demonstrates how to read sales records from a CSV file, clean numeric values, calculate revenue, rank products, identify high-value transactions, and verify results with Pandas.

## Dataset
The analysis uses `electronics_sales.csv`, containing 50 sales records dated from 1 September 2026 to 30 September 2026.

The source columns are:
- `sale_id` — unique sales reference
- `sale_date` — date of the transaction
- `store` — store location
- `product` — product sold
- `quantity` — number of units sold
- `unit_price_kes` — unit price in Kenyan shillings
- `payment_method` — payment method used

## Tools and Concepts
- Python
- `csv` module and `csv.DictReader`
- Dictionaries and lists
- Data cleaning and numeric type conversion
- Loops, conditional logic, and list comprehensions
- Functions for mean, median, and minimum/maximum
- Revenue aggregation by product and store
- Pandas for independent verification

## Key Findings
- **Total revenue:** KES 1,310,812.00
- **Number of sales records:** 50
- **Top product by revenue:** HP 15 Laptop — KES 389,994.00
- **Second-highest product:** Hisense 43in Smart TV — KES 272,993.00
- **Third-highest product:** Lenovo Tab M10 — KES 199,992.00
- **High-value transactions:** 3 transactions of KES 100,000 or more
- **Verification:** The notebook's manual revenue calculation matched the Pandas total.

## How to Run
1. Place `electronics_sales.csv` in the project's `Data/` folder.
2. Open `Day2.ipynb` in Jupyter Notebook or VS Code with a Python/Jupyter environment.
3. Update the CSV file path in the notebook to match your local folder structure.
4. Run the notebook cells from top to bottom.

Pandas is required for the verification section. Install was needed `pip install pandas`.


## Notes and Limitations
- The dataset contains transaction details, but the notebook's current analysis does not calculate profit because cost data is not included.
- Product and store totals represent revenue calculated from quantity multiplied by unit price; no discounts were present in the displayed records.
- Keeping the dataset path relative where possible so the project can run on other computers.

## Project Purpose
This is a practical Python data-analysis exercise focused on file handling, data cleaning, reusable functions, aggregation, and result validation.
