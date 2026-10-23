# Retail Sales Dashboard — Explained for Everyone

**A simple, visual way to explore retail sales.** This project presents example sales information in a modern dashboard with summary numbers, charts, and comparisons.

## 👀 See the dashboard

- **Open the dashboard website:** [View Sales Pulse](https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/)
- **See the HTML source code:** [Open `index.html`](./index.html)
- **See all project files:** [Browse this repository](https://github.com/ganesh9193singh-sketch/Retail-Glassmorphism-Dashboard)

> If the dashboard website does not open yet, GitHub Pages may not be enabled for this repository. Follow the publishing steps below. The HTML file can still be opened directly from GitHub using the source-code link, but GitHub's file viewer is not the same as running the dashboard website.

## What is this project?

Imagine a shop owner who wants to answer questions such as:
- How much money did the shop make from orders that were delivered?
- How much profit did those orders generate?
- Which sales channel appears to perform best?
- Which region has the highest sales?
- How many orders were delivered, returned, or cancelled?

Instead of checking many rows in a spreadsheet, a dashboard puts important information into one place. The charts make it easier to spot patterns quickly.

## What do the words mean?

- **Dashboard:** one screen that summarizes important information.
- **KPI (Key Performance Indicator):** a number used to understand performance, such as sales or profit.
- **Sales:** the amount recorded from selling products. Sales are not the same as profit.
- **Profit:** the amount left after the costs represented in the data are accounted for.
- **Average order value:** delivered sales divided by the number of delivered orders.
- **Sales channel:** the way a customer places an order, such as online, by phone, or in a store.
- **Region:** the geographical area associated with a customer.
- **HTML:** the structure of a web page.
- **CSS:** the rules that control the page's appearance, such as colors, spacing, and layout.
- **JavaScript:** the code that makes parts of a page interactive.
- **Power BI:** Microsoft's tool for building reports and dashboards from data.

## What can you see in the dashboard?

1. **Delivered sales** — the total sales amount for orders marked as delivered.
2. **Delivered profit** — profit for orders marked as delivered.
3. **Delivered orders** — how many orders have the Delivered status.
4. **Average order value** — average delivered sales per delivered order.
5. **Monthly sales chart** — helps compare sales across months.
6. **Sales by channel** — compares online, phone, and store sales.
7. **Sales by region** — compares the sales amounts associated with different regions.
8. **Order status mix** — shows delivered, returned, and cancelled orders.

The channel buttons are part of the HTML demo. Review the underlying data and calculation logic before using these visuals as business reporting.

## How is it built?

This repository contains a **web dashboard** and supporting files for a separate **Power BI report**.

- `index.html` — the web dashboard. It contains the HTML, CSS, and JavaScript in one file, so no framework installation is needed to understand or open the source.
- `powerbi/GlassmorphismTheme.json` — a theme file for Power BI that sets a dark background and a coordinated set of colors.
- `powerbi/DAX_Measures.txt` — example formulas for calculating sales, profit, order counts, and other metrics in Power BI.
- `powerbi/README.md` — a beginner-friendly guide to using the Power BI files.
- `.github/workflows/deploy.yml` — an automation recipe intended to publish the website through GitHub Pages.

**Important:** An HTML dashboard is not a Power BI report file. This repository does not currently contain a finished `.pbix` report or a public Power BI Service report link. The Power BI theme and DAX formulas are starter materials that can be used to build a report in Power BI Desktop.

## How to run the HTML dashboard on your computer

1. Open the [`index.html` file](./index.html).
2. On GitHub, use the download option to save the file to your computer (or clone/download the repository).
3. Open `index.html` in a modern browser such as Chrome or Edge.

The web dashboard is a static demo and does not need a server or an API to open locally.

## How to publish it so anyone can view it

1. Open this repository's **Settings**.
2. Select **Pages** from the sidebar.
3. Under the build/deployment settings, choose **GitHub Actions** as the source if it is available.
4. Open the **Actions** tab and check the “Deploy static dashboard to GitHub Pages” workflow.
5. After a successful deployment, visit: [https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/](https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/)

The workflow may not be able to configure Pages automatically if Pages has not been enabled for the repository. If the run fails, enable Pages in Settings and re-run the workflow.

## How to build the Power BI report

1. Install and open Power BI Desktop.
2. Import the customer, order, and product CSV files (when they have been added to the repository).
3. Connect customer IDs between the Customers and Orders tables, and product IDs between Products and Orders.
4. Import the theme using **View → Themes → Browse for themes** and select `powerbi/GlassmorphismTheme.json`.
5. Create measures from `powerbi/DAX_Measures.txt`, checking that the column names match the data you imported.
6. Add cards, bar charts, and slicers to create your report.
7. Save your report as a `.pbix` file.

The CSV data files are not currently included in this repository, so the Power BI instructions are a guide, not a ready-to-open report.

## Data and accuracy note

The dashboard includes demonstration figures. Treat them as sample data, not verified company results. Some visual summaries are illustrative and should be checked against the source data before making decisions. Do not use the figures for financial or business decisions without validating them.

## Design and AI disclosure

AI tools were used as an aid during visual design exploration and graphic styling, including ideas for the glassmorphism effect, color palette, and visual presentation. The project should be tested and reviewed by its author, and all metrics should be checked against the source data.

## Project structure

```
Retail-Glassmorphism-Dashboard/
├── index.html
├── README.md
├── powerbi/
│   ├── DAX_Measures.txt
│   ├── GlassmorphismTheme.json
│   └── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

## Next improvements

- Add the validated customer, order, and product CSV files.
- Build and include a Power BI `.pbix` report.
- Validate all dashboard figures and connect the channel filters to real underlying data.
- Publish the HTML site and, separately, publish a Power BI report if a shareable Power BI link is needed.
