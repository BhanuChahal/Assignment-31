# L0: MongoDB Aggregations - Sales Data Analysis

## Files
- `sales.json` → dataset for the `sales` collection
- `queries.txt` → all aggregation pipelines

## Setup
```bash
use masai

# Import the dataset
mongoimport --db masai --collection sales --file sales.json --jsonArray
```

## Verify data
```bash
db.sales.find().pretty()
```

## Run aggregations
Copy-paste each pipeline from `queries.txt` into the Mongo Shell or use Compass Aggregation tab.

Each query corresponds to a task:
1. Total sales per category
2. Month-wise total sales
3. Highest-selling product
4. Average sale amount
5. Monthly sales count
6. Regional total sales
7. Top 3 products by revenue
8. Transaction count per category
9. Regional average sales
10. Category-wise totals for Electronics and Fashion
