# Power BI Guide — Beginner Friendly

This folder contains starter files to help you build a report in Microsoft Power BI. It does **not** contain a finished Power BI report yet.

## Start here

- **[Open the separate HTML dashboard demo](https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/)**
- **[View the dashboard's HTML source code](../index.html)**
- **[Open the Power BI embed HTML template](./embed-template.html)**

The HTML dashboard is a working-style web demo. It is not itself a Power BI report, and an HTML link cannot automatically turn into a Power BI report.

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

## How to make a real Power BI report link

1. Open Power BI Desktop and import your data.
2. Apply the theme and create charts and measures.
3. Save the report as a `.pbix` file.
4. Publish it to Power BI Service, if your account supports publishing.
5. Use the report's supported sharing/embed option and check access permissions.
6. If you want to display it inside a webpage, copy the authorized embed URL into `embed-template.html`, replacing `REPLACE_WITH_YOUR_POWER_BI_EMBED_URL`.

**Important:** This repository does not currently contain a finished `.pbix` report or a real Power BI Service report link. The template cannot show a Power BI report until you publish one and insert its real embed URL. Avoid public embedding for private or sensitive data.

## HTML dashboard versus Power BI

- **HTML dashboard demo:** [Open the web dashboard](https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/)
- **HTML code:** [Open `index.html`](../index.html)
- **Power BI embed template:** [Open `embed-template.html`](./embed-template.html)

These are two separate outputs. The website can be published using GitHub Pages. A Power BI report must be created and published separately in Power BI.
