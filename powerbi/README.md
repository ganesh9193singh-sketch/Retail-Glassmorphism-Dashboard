# Power BI Starter Guide

This folder contains starter resources for creating a retail analytics report in Microsoft Power BI. **It does not contain a finished Power BI `.pbix` report or a published Power BI report URL.**

## Project links

- **Live HTML dashboard:** https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/
- **Main dashboard HTML source:** [Retail-Glassmorphism-Command-Center (1).html](../Retail-Glassmorphism-Command-Center%20(1).html)
- **Website entry point:** [index.html](../index.html)
- **Power BI embed template:** [embed-template.html](./embed-template.html)
- **Main project README:** [README.md](../README.md)

The HTML dashboard and a Power BI report are separate deliverables. Publishing the HTML website does not create or publish a Power BI report.

## Files in this folder

### `GlassmorphismTheme.json`

A Power BI theme file that sets a consistent visual style for report pages and visuals.

**Import the theme**
1. Open Power BI Desktop.
2. Select **View → Themes → Browse for themes**.
3. Choose `GlassmorphismTheme.json`.

Review the result in Power BI and adjust colors or formatting as needed.

### `DAX_Measures.txt`

A collection of example DAX measure notes. Treat them as starter formulas, not validated financial definitions.

**Use the formulas**
1. Import your own dataset into Power BI.
2. Check that table and column names match the formulas.
3. Create each measure using **Modeling → New measure**.
4. Adjust the formula for your data model and order-status rules.
5. Compare the results with manual calculations and trusted source totals.

### `embed-template.html`

A basic HTML template for displaying a Power BI report after you have a valid report embed URL and the correct permissions. It is not a report and will not work with a placeholder URL.

## Data requirements

The precise schema depends on your source data and the measures you choose. A typical retail model may include:

- **Orders:** order ID, date, customer ID, product ID, quantity, sales amount, cost/profit fields, and order status.
- **Customers:** customer ID and appropriate customer attributes, such as region.
- **Products:** product ID, product name, and category.

Use stable IDs to define relationships. Confirm data types, duplicate keys, missing values, currency, date ranges, and order-status definitions before building visuals.

**Data availability:** There are no dedicated CSV data files listed in this repository at present. Add or connect the appropriate source data before expecting a populated Power BI report.

## Create and embed a Power BI report

1. Open Power BI Desktop and import your data.
2. Build and validate your data model, relationships, measures, and visuals.
3. Save the report as a `.pbix` file.
4. Publish it to Power BI Service if your account and organization allow it.
5. Choose an appropriate sharing or embed method and confirm the access permissions.
6. Replace `REPLACE_WITH_YOUR_POWER_BI_EMBED_URL` in `embed-template.html` with the authorized embed URL, if that template suits your use case.
7. Test the page while signed in and, where relevant, with a viewer account that has the intended permissions.

Do not publicly embed private, confidential, or personal data. Public publishing can make report data accessible to anyone with the link or through the public web.

## Validate before presenting results

- Confirm the source and refresh date.
- Document how sales, profit, delivered orders, returns, cancellations, and AOV are calculated.
- Check totals against the original records.
- Verify access permissions for any published report.
- Clearly label sample or illustrative data.

