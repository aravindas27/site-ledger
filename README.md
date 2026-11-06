# Construction Site Ledger

A dashboard for the construction business accounts. It reads the master Excel file
(`Construction_Accounts_Site_Costing.xlsx`) and shows:

- Money on hand: balance in each bank account and in cash, plus total funds
- Money received and spent in any period (all time, this month, last month, last 7 days, or chosen dates)
- Project costing for each site: received, cost, profit or loss, and the cost split into
  material, labour, subcontract, machinery and other costs. Tap a site to see every entry for it.
- All entries, with filters by site, account, type and a search box
- Month-by-month totals
- Office and personal spending
- Entries that still need fixing in Excel (missing date, site, category or account)

## Data on this site

`data.json` holds the current figures exported from the master Excel file, and the dashboard
opens with them. **This repository and website are public**, so anyone with the link can see
these figures.

To refresh the site, export the latest Excel into `data.json` and push it. For a one-off look at
newer entries, tap **Open Excel file** on the page: that file is read only on your device and is
never uploaded.

## Publishing on GitHub Pages

1. Create a new repository on GitHub (for example `site-ledger`).
2. Upload `index.html` (and this README) to the repository.
   Do **not** upload the Excel file: GitHub Pages sites are public.
3. Go to **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, then click **Save**.
4. After a minute the dashboard is live at `https://<your-username>.github.io/site-ledger/`.

## Daily use

1. Enter the day's transactions in the **Transactions** sheet of the Excel file and save it.
2. Open the dashboard link and click **Open Excel file**, or drag the file onto the page.
