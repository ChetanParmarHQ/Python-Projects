# E-Commerce Database Analysis

An exploratory data analysis (EDA) project on the Superstore retail dataset, built with Python. It breaks down sales, profit, customer segments, and profitability ratios to turn raw order data into clear business insights.

Maintained by **Chetan Parmar**.

---

## Project overview

Using a real world style e-commerce dataset of nearly 10,000 orders, this project answers practical questions a retail business would ask: when do we sell the most, which categories and products drive revenue, which ones lose money, and which customer segments are the most profitable.

The analysis uses interactive Plotly charts to visualise monthly trends, category breakdowns, and segment comparisons.

---

## Dataset

| Detail | Value |
|--------|-------|
| File | `Superstore.csv` |
| Rows | 9,994 orders |
| Columns | 21 |
| Period | 2014 to 2017 |

**Key columns:** Order Date, Ship Date, Ship Mode, Segment, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit

---

## Questions answered

1. Which month had the highest and lowest sales?
2. Which product category has the highest and lowest sales?
3. How do sales break down by sub-category?
4. Which month had the highest and lowest profit?
5. How does profit split across categories and sub-categories?
6. Which customer segment performs best on sales and profit?
7. What does the sales to profit ratio reveal about profitability?

---

## Key findings

**Sales**
- Highest sales month: November (about 352,461).
- Lowest sales month: February (about 59,751).
- Highest sales category: Technology (about 836,154, roughly 36 percent).
- Lowest sales category: Office Supplies (about 719,047, roughly 31 percent).
- Top selling sub-category: Phones (about 330,007). Lowest: Fasteners (about 3,024).

**Profit**
- Highest profit month: December (about 43,369). Lowest: January (about 9,134).
- Highest profit category: Technology (about 145,455, roughly 51 percent).
- Lowest profit category: Furniture (about 18,451, roughly 6 percent).
- Best profit sub-category: Copiers (about 55,618).
- Loss making sub-category: Tables (about -17,725).

**Segments and profitability**
- Consumer is the top segment for both sales and profit; Home Office is the smallest.
- Sales to profit ratio (lower is better): Technology is the most profitable category, while Furniture is the least.
- Tables, Bookcases, and Supplies stand out as the least profitable sub-categories, some running at a loss.

---

## Analysis steps

1. Loaded the Superstore data with latin-1 encoding.
2. Converted `Order Date` and `Ship Date` to datetime.
3. Extracted order month, year, and day of week for time based analysis.
4. Grouped and aggregated sales and profit by month, category, sub-category, and segment.
5. Calculated the sales to profit ratio at each level.
6. Visualised results with line charts, bar charts, and donut pie charts.

---

## Tools and libraries

- **Language:** Python 3
- **Libraries:** pandas, NumPy, Plotly (express and graph_objects)
- **Environment:** Jupyter Notebook / Google Colab

---

## Repository contents

```
E-Commerce Database Analysis/
|-- E_commerce_Database_Analysis.ipynb   # Full analysis notebook
|-- Superstore.csv                       # Source dataset
|-- E-Commerce Database Analysis.pdf     # Project brief and presentation
|-- README.md                            # You are here
```

---

## How to run

1. Clone the repository and open the folder.
2. Install the libraries:
   ```bash
   pip install pandas numpy plotly
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook E_commerce_Database_Analysis.ipynb
   ```
   Or open it directly in Google Colab.
4. Run the cells top to bottom. The notebook downloads the dataset automatically if `Superstore.csv` is not present.

---

## Author

**Chetan Parmar**

GitHub: [@ChetanParmarHQ](https://github.com/ChetanParmarHQ)

---

*This project is part of a wider Python portfolio focused on data analysis and real-world problem solving.*

