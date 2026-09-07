# Day 15: Product Count Analysis

## Objective
Practice aggregate functions by counting products by category and identifying the largest category within a retail dataset, ensuring accurate inventory representation.

## Technical Implementation
To accurately count the product catalog, I had to differentiate between *transaction counts* (how many times an item was sold) and *unique product counts* (how many distinct items exist in the catalog).

1. **Data Isolation:** Engineered a two-tab structure to separate raw sales data from the active analysis dashboard.
2. **Unique Extraction:** Implemented the `=UNIQUE()` function to extract a clean list of distinct products and their associated categories, successfully filtering out duplicate sales transactions (e.g., multiple orders of the same 'Desk Chair').
3. **Categorical Aggregation:** Utilized the `=COUNTIF()` function on the cleaned unique list to tally the exact number of individual products belonging to each category.

## Findings & Deliverables
* **Top Category:** The largest category by unique product count is **Supplies**.
* **Product Count Table:**
  * Supplies: 3 unique products
  * Tech: 2 unique products
  * Furniture: 1 unique product
