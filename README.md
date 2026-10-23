# Retail Sales Dashboard — Glassmorphism Command Center

A retail-sales analytics portfolio project focused on a polished glassmorphism visual style and business-focused KPIs.

## Project status
The dashboard source and supporting project files are being organized for this repository. The visual design uses a dark navy background, frosted-glass panels, and cyan, emerald, violet, and rose accents.

## Design and AI disclosure
AI tools were used as an aid during visual design exploration and graphic styling, including ideas for the glassmorphism treatment, color palette, and presentation polish. The project should be reviewed, tested, and understood by its author before being presented as finished work.

## Planned repository structure
- `index.html` — interactive dashboard
- `data/` — source CSV files for customers, orders, and products
- `powerbi/` — Power BI theme and DAX measures / project files
- `.github/workflows/deploy.yml` — GitHub Pages deployment workflow

## Dashboard concepts
- Executive KPIs: net sales, net profit, order leakage, and average order value
- Product and customer insights
- Regional and channel comparisons
- Gross versus delivered-order (net) sales analysis

## Power BI notes
Import the customer, order, and product CSV files into Power BI Desktop, create the relationships using customer and product IDs, then apply the theme JSON and add the DAX measures.

## GitHub Pages
The included workflow publishes the repository root using GitHub Actions when the required dashboard file is present. In GitHub, open **Settings → Pages** and select **GitHub Actions** as the deployment source.

## Data note
Treat the included data as demonstration data unless its provenance has been independently verified. Validate all measures and figures before using them for business decisions.
