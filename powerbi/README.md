# Power BI Guide — Beginner Friendly

This folder contains starter files to help you build a report in Microsoft Power BI. It does **not** contain a finished Power BI report yet.

## Files in this folder

### `GlassmorphismTheme.json`
A theme is like a design preset. It gives charts and report pages a consistent color style, including a dark background and bright accent colors.

**How to apply it**
1. Open Power BI Desktop.
2. Open the **View** tab.
3. Choose **Themes → Browse for themes**.
4. Select `GlassmorphismTheme.json`.

### `DAX_Measures.txt`
This file contains example formulas. In Power BI, formulas are called DAX measures. They calculate values such as delivered sales, profit, delivered orders, and average order value.

**How to use the formulas**
1. Import your data into Power BI.
2. Confirm that your table and column names match the formulas.
3. Create a measure from the **Modeling → New measure** option.
4. Copy one formula at a time and adjust it to match your data.
5. Check the results against a manual calculation before trusting the report.

## Data needed

A typical version of this project needs three tables:
- **Customers:** one row per customer, including a customer ID and region.
- **Orders:** one row per order, including customer ID, product ID, date, sales, profit, and order status.
- **Products:** one row per product, including a product ID and product name/category.

Connect the tables using the matching IDs. The CSV files are not currently included in this repository, so you will need to add the correct source data before building the full report.

## HTML dashboard versus Power BI

The website preview is a separate HTML dashboard:
[View the HTML dashboard](https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/)

Its source code is here:
[Open index.html](../index.html)

Power BI Desktop creates a separate report file with the `.pbix` extension. To share a live Power BI report, you must create the report, publish it to Power BI Service, and use an authorized sharing link. A normal HTML URL cannot automatically become a Power BI report.

## Before sharing
- Validate the data and formulas.
- Remove confidential information.
- Check the report's sharing permissions.
- Remember that publishing to Power BI Service may depend on your account, organization settings, and licensing.
