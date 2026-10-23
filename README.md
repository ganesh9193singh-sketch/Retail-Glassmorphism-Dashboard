# Retail Glassmorphism Command Center

A browser-based retail analytics dashboard with a dark glassmorphism interface. The project is designed to present retail KPIs and exploratory views for sales, profit, orders, products, customers, regions, and sales channels.

> **Important:** This is a demonstration/learning project. Do not treat displayed figures as verified business results unless you validate the underlying data and calculations.

## Open the dashboard

- **Live website:** https://ganesh9193singh-sketch.github.io/Retail-Glassmorphism-Dashboard/
- **Dashboard HTML source:** [Retail-Glassmorphism-Command-Center (1).html](./Retail-Glassmorphism-Command-Center%20(1).html)
- **GitHub repository:** https://github.com/ganesh9193singh-sketch/Retail-Glassmorphism-Dashboard
- **Deployment workflow:** [deploy.yml](./.github/workflows/deploy.yml)

If the live site does not update immediately after a commit, check the repository's **Actions** tab for the GitHub Pages deployment and wait for it to finish. Then refresh the site, or try a hard refresh.

## Project overview

The dashboard's purpose is to make retail performance easier to explore in one place. Depending on the dashboard version and available data, its views may cover:

- Sales and revenue trends
- Profitability indicators
- Order status and returned/cancelled orders
- Average order value (AOV)
- Product and category performance
- Customer segments
- Regional performance
- Sales channels and payment methods

These are analysis views, not proof of the causes behind a business change. Investigate source records and business context before making decisions.

## Dashboard areas

### Executive Overview — Pulse
A high-level view intended to summarize important performance indicators and compare trends or segments.

### Product & Customer Insights — Microscope
A deeper exploration area intended to examine product/category results, customer mix, and order/payment patterns.

The exact visuals, labels, filters, interactions, formulas, and figures are determined by the current HTML file. Check the dashboard itself and its source code before relying on a particular metric.

## Key metric definitions

The following are common interpretations; the actual formula implemented in this project should be checked before reporting results.

| Metric | General meaning |
|---|---|
| Gross Sales | Sales value before any exclusions defined by the business. |
| Net Sales | Sales after applying the project's chosen exclusions or adjustments. |
| Net Profit | Sales minus the costs included in the calculation; this is not necessarily full accounting profit. |
| Order Leakage % | A defined share of orders that do not reach the desired completed state, such as returned or cancelled orders. Confirm the denominator and statuses used. |
| Average Order Value (AOV) | Sales value divided by the order count selected by the metric definition. |

**Metric validation checklist**
1. Identify the data source and refresh date.
2. Confirm currency, date range, and whether amounts include tax, discounts, shipping, or returns.
3. Confirm which order statuses are included in each measure.
4. Reconcile totals with source records or trusted reports.
5. Document the exact formula before presenting figures.

## Technology and design

- Static HTML entry point for GitHub Pages.
- Dark, glassmorphism-inspired visual design with translucent panels and accent colors.
- Intended to be viewed in a modern desktop or mobile browser.
- GitHub Actions workflow deploys the repository contents to GitHub Pages when changes are pushed to `main`, or when manually triggered.

The dashboard is hosted as a static site. No live database connection is confirmed by the repository structure alone; inspect the HTML and any data-loading code to establish whether values are embedded, sample values, or loaded from another source.

## Repository structure

```text
.
├── index.html
├── Retail-Glassmorphism-Command-Center (1).html
├── .github/
│   └── workflows/
│       └── deploy.yml
└── powerbi/
    ├── DAX_Measures.txt
    ├── GlassmorphismTheme.json
    ├── README.md
    └── embed-template.html
```

- **`index.html`** — site entry point that redirects visitors to the dashboard HTML file.
- **`Retail-Glassmorphism-Command-Center (1).html`** — main dashboard page.
- **`.github/workflows/deploy.yml`** — GitHub Actions workflow for publishing the static site.
- **`powerbi/`** — Power BI theme and starter documentation/resources.
- **Data files** — no dedicated top-level `data/` directory is currently listed in the repository. Do not assume external or live retail data is connected without checking the dashboard implementation.

## Run locally

1. Open the repository and select **Code → Download ZIP**, or clone it:
   ```bash
   git clone https://github.com/ganesh9193singh-sketch/Retail-Glassmorphism-Dashboard.git
   ```
2. Open `index.html` in a modern browser. If the redirect does not work in your local file viewer, open `Retail-Glassmorphism-Command-Center (1).html` directly.
3. To publish a change, commit it to the `main` branch.
4. Open the **Actions** tab and confirm that the **Deploy static dashboard to GitHub Pages** workflow succeeds.

Because the page is static, it does not require a backend server unless you add features that depend on one. Any external assets or data sources used by the page must still be reachable.

## Power BI resources

The `powerbi/` directory contains supporting starter resources:

- `GlassmorphismTheme.json` — a theme file for Power BI.
- `DAX_Measures.txt` — example/working notes for DAX measures; verify the formulas against your model.
- `embed-template.html` — a template that requires a valid Power BI report embed URL and appropriate sharing/access settings.
- `README.md` — instructions for the Power BI resources.

These files do not, by themselves, mean a published Power BI report is embedded or connected to the live website.

## Limitations and responsible use

- Demo or embedded values may not represent current real-world sales.
- Formulas can differ from standard business definitions; validate them in the code or Power BI model.
- No guarantee is made that a live retail database, automatic refresh, authentication, or a production backend is configured.
- Do not use unverified dashboard values for accounting, tax, inventory purchasing, or other high-impact business decisions.
- Review and test changes before presenting the project as production-ready.

## Contributing / improving the project

For a useful improvement, include:
- A clear description of the change.
- Screenshots for significant visual changes.
- The data source and formula definitions for new metrics.
- Testing notes, including browser/device and whether the Pages deployment succeeded.

---

Created as a retail analytics learning project focused on a glassmorphism command-center interface.
