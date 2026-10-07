# Mobile Sales: Mini EDA

Exploratory data analysis of a mobile phone sales dataset (about 3,800 transactions), completed as Project
## Dataset
`mobile_sales_project.csv` contains sales transactions with order date, brand, model, units sold, price, total, customer details, city, payment method and customer ratings.

## What I did
- **Loaded and inspected** the data with `head`, `tail`, `info`, `describe` and `dtypes`.
- **Cleaned the data:**
  - Filled missing numeric values (Units Sold, Price Per Unit, Customer Ratings) with the median, because the data contains outliers.
  - Filled missing categories (City, Payment Method) with the most common value.
  - Dropped 5 rows with no Customer Name.
  - Converted `Order Date` to datetime.
  - Removed 9 duplicate rows.
- **Explored** the data with `value_counts`, `groupby` and `describe`.
- **Visualised** it with a histogram, a boxplot and a bar chart.
- **Wrote 3 insights** in Observation → Insight → Action format.

## Key findings
- Delhi and Mumbai account for about 43% of orders and sales, but they are only 2 of the 19 cities.
- Sales are spread evenly across brands. Apple has the highest average order value, about 8% above Xiaomi.
- The raw data had unrealistic values (such as a customer aged 150 and a 2.25 million order), so cleaning and checking was needed before analysis.

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn (Google Colab / Jupyter Notebook)

## How to run
1. Download `Project1_Mini_EDA.ipynb` and `mobile_sales_project.csv` into the same folder.
2. Open the notebook in Jupyter or Google Colab (upload the CSV in Colab).
3. Run all cells from top to bottom.
