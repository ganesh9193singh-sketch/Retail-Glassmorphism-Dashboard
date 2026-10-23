# Retail Glassmorphism Command Center

A modern, dark-mode retail analytics dashboard designed to help people understand sales performance, profitability, customer activity, and order issues at a glance. It uses a glassmorphism visual style: translucent panels, soft borders, and bright accent colors.

## Open the project

- **GitHub repository:** https://github.com/ganesh9193singh-sketch/Retail-Glassmorphism-Dashboard

> The published website displays the dashboard version currently committed as index.html. Treat figures as demo analytics unless the supplied data files are connected and verified.

## What the dashboard is for

Retail businesses can use a dashboard like this to monitor:
- **Sales:** revenue generated over time.
- **Profit:** what remains after the costs represented in the dataset.
- **Order leakage:** the share of orders returned or cancelled instead of successfully delivered.
- **Average order value (AOV):** average sales value per delivered order.
- **Regions and channels:** how performance differs across regions, payment methods, and sales channels.
- **Products and customers:** which categories, products, and customer groups contribute to performance.

These views help teams spot changes, compare segments, and decide what to investigate. They do not by themselves prove why a change happened.

## Dashboard sections

### 1. Executive Overview — Pulse
A high-level view for checking key performance indicators, revenue trends, geographic performance, and channel/payment comparisons.

### 2. Product & Customer Insights — Microscope
A deeper view for exploring category profitability, customer mix, product rankings, and payment/order-status patterns.

The exact values, chart availability, filters, and interactions depend on the version of index.html and the data embedded or connected to it.

## Design and accessibility

- **Style:** glassmorphism panels on a deep navy/charcoal background.
- **Accent colors:** cyan for sales, green for profit, violet for costs, and rose for alerts.
- **Typography:** sans-serif text.
- **Charts:** interactive chart elements may show more detail on hover or selection.
- **Layout:** designed to adapt to common desktop and smaller screens.

## Understanding the key metrics

| Metric | Plain-English meaning |
|---|---|
| Gross Sales | Total sales value before excluding returned or cancelled orders. |
| Net Sales | Sales counted for delivered orders under the project's stated rule. |
| Net Profit | Profit calculated using the project's available sales and cost logic. Confirm the exact formula before reporting it. |
| Order Leakage % | Returned and cancelled orders divided by all orders. |
| Average Order Value (AOV) | Net sales divided by the number of delivered orders. |

Metric definitions are only as reliable as the underlying data and implementation. Check the dashboard code or Power BI measures before using numbers for business decisions.

## Data and limitations

The dashboard interface does not guarantee that a live retail database is connected. Check the repository's data folder and the dashboard's data-loading code to confirm which files are present and used. Embedded sample data is illustrative, not a verified current business result.

Do not use demo numbers for accounting, tax, inventory purchasing, or other important decisions without validating them against original records.

## Run it locally

1. Download or clone this repository.
2. Open index.html in a modern browser.
3. To publish changes, commit them to the main branch. The GitHub Actions workflow in .github/workflows/deploy.yml publishes the site through GitHub Pages.

A self-contained static HTML dashboard does not need a backend server. Any external assets or data files it depends on must also be available.

## Power BI resources

The powerbi/ folder contains supporting Power BI materials such as a theme, DAX measure notes, and an embed template. These are separate from the website. The embed template needs a real Power BI report embed URL; it is not itself a hosted Power BI report.

## Repository structure

- index.html — website entry point served by GitHub Pages.
- .github/workflows/deploy.yml — automatic GitHub Pages deployment workflow.
- powerbi/ — Power BI theme, measure notes, and related starter resources.
- data/ — retail data files, if present in this repository.

## AI and project transparency

This project is an analytics demonstration. AI-assisted code or documentation should be reviewed and tested by a person. Verify formulas, source data, and chart behavior before presenting results as business facts.

---
Built as a retail analytics learning project with a glassmorphism command-center design.
