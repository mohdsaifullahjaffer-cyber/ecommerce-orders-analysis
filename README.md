# E-commerce Orders Analysis

A Python and SQL portfolio project exploring 10,000 e-commerce orders, with a focus on delivered sales and order statuses.

## Tools

Python, pandas, Matplotlib, SQLite, and Jupyter Notebook. SQLite is included with Python.

## Analysis

- Missing-value, duplicate-row, order-ID, and date checks
- Delivered sales totals and average order value
- Category and product sales, payment methods, and country summaries
- Monthly delivered sales chart and date-coverage checks
- Order status chart
- SQL aggregations for category sales, total sales, top products, and monthly trends

## Key Results

| Metric | Result |
| --- | ---: |
| Delivered orders | 2,037 |
| Delivered sales value | 1,582,371 |
| Average delivered order value | 776.81 |
| Highest monthly delivered sales | 73,792 (August 2024) |

Electronics led delivered category sales at 1,002,864. Samsung Galaxy S23 led product sales at 427,924. These figures come from the notebook's saved outputs.

Dataset coverage runs from August 25, 2022 through August 24, 2025. August 2022 and August 2025 are partial months. Order statuses are fairly evenly distributed.

## Run Locally

1. Download this repository's notebook and `requirements.txt` into a project folder.
2. Place `ecommerce_dataset_10000.csv` in the same folder.
3. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `ecommerce_orders_analysis.ipynb`, restart the kernel, and run all cells in order.

The SQLite database is temporary and rebuilt within the notebook.

## Data Source

The input filename is `ecommerce_dataset_10000.csv`. The original dataset URL and license were not supplied. Add the source link and license before publishing or redistributing the dataset. The CSV is not included in these deliverables.

## Definitions and Limitations

Sales value equals quantity multiplied by unit price for delivered orders only. It does not represent profit and does not separately account for discounts, taxes, or shipping. Currency is unconfirmed. Partial months require care when comparing monthly totals. The dataset alone does not explain why sales changed.

## Validation Status

The cleaned notebook passed notebook-structure and Python-syntax checks. Saved outputs were retained from the original notebook; the cleaned version has not been executed against the source CSV because it was not attached. Run all cells with the CSV before publishing.
