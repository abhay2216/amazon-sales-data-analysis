# Amazon Sales Data Analysis

A data analysis project on Amazon.in sales data (31 March to 29 June 2022), completed as **Project 78G0OL** of a Data Analyst internship. It uses Python for cleaning and analysis, and Power BI for an interactive dashboard.

## What the project does

The project turns 128,976 raw order lines into findings and recommendations on:

- **Sales trends** over time
- **Products:** categories, sizes and quantities
- **Fulfilment:** Amazon versus Merchant, including cancellations
- **Customer groups:** business versus regular buyers, and spending groups
- **Regions:** sales and cancellations by state and city

## Tech stack

| Tool | Used for |
|---|---|
| Python 3 | Data cleaning and analysis |
| pandas | Loading, cleaning, grouping and calculations |
| matplotlib | Charts saved as images |
| VS Code + Jupyter Notebook | Writing and running the code |
| Power BI Desktop (DAX, Power Query) | Interactive dashboard and measures |
| CSV | Raw and cleaned data files |
| Microsoft Word | Report and documentation |

## How it works

1. **Collect:** start from one CSV file of Amazon orders.
2. **Clean:** pandas fixes dates and spellings, standardises state names, drops empty columns and keeps cancelled orders apart from sales. The result is saved as a cleaned CSV.
3. **Analyse:** the notebook groups the data by month, product, size, fulfilment method and state, and saves the charts.
4. **Dashboard:** the cleaned CSV is loaded into Power BI, where DAX measures and slicers make a two-page interactive dashboard.
5. **Report:** findings and recommendations are written up in Word.

## Dashboard

- **Page 1, Sales Overview:** revenue, orders, items sold, average order value, cancellation rate, monthly and daily revenue, revenue by category, items sold by size.
- **Page 2, Fulfilment and Regions:** cancel rates by fulfilment method, return rate, revenue shares, order status, spending groups, cancellation by state, top 10 states and cities.

Slicers for month, category, fulfilment method and buyer type update every chart.

## Key results

- Revenue of **₹71.7 million** from 100,600 orders (average order ₹712).
- T-shirts, Shirts and Blazers bring in **91%** of revenue.
- Monthly sales fell from ₹26.2M in April to ₹21.4M in June.
- Merchant-fulfilled orders are cancelled more often (**17.5%**) than Amazon-fulfilled orders (**12.8%**).
- Maharashtra, Karnataka and Telangana give **39%** of revenue.

## Project files

| File or folder | Description |
|---|---|
| `Project.ipynb` | Python notebook with the cleaning and analysis code |
| `Amazon Sale Dataset.csv` | Raw dataset |
| `charts/` | Saved chart images |
| `tables/` | Summary tables and key numbers |
| `Power BI Amazon Sales Dashboard/` | The Power BI dashboard (`Amazon_Sales_Dashboard.pbix`, open with Power BI Desktop) and the cleaned dataset it uses (`Amazon_Sales_Clean_Dataset.csv`) |
| `Project Report/` | Full analysis report (Word and PDF) |
| `Project Documentation/` | Project documentation (Word and PDF) |

## How to run

```bash
pip install pandas matplotlib jupyter ipykernel
```

1. Keep `Amazon Sale Dataset.csv` in the same folder as the notebook.
2. Open `Project.ipynb` in VS Code (or Jupyter) and run the cells from top to bottom, once each.
3. Open `Amazon_Sales_Dashboard.pbix` in Power BI Desktop to explore the dashboard. It reads the cleaned dataset from the same folder.

## Author

Abhay Sharma
