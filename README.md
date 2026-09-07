# Duty & Interest Ledger

A single-page, browser-based ledger for tracking monthly dues, arrears, interest, and payments. No backend, no build step, no database — it's one self-contained HTML file that runs entirely in the browser.

**Live app:** _(add your GitHub Pages link here once deployed, e.g. `https://YOUR-USERNAME.github.io/duty-interest-ledger/`)_

## How it works

- All calculations happen client-side in JavaScript.
- Your data is **not** sent to any server. Nothing is stored remotely.
- Use the **Save Ledger** button (in the settings drawer) to download your data as a `.json` file, and **Import Saved Ledger** to reload it later. Save regularly — closing the tab without saving loses unsaved changes.
- The **Complete Report** tab can be turned into a PDF using its **Save as PDF** button (uses your browser's print dialog).

## Deploying to GitHub Pages (free hosting)



## Notes

- The file loads one external script (SheetJS, for Excel export) from a public CDN (`cdnjs.cloudflare.com`). No API keys or accounts are required for this.
- Because everything runs client-side, GitHub Pages' free static hosting is sufficient — no server, database, or paid plan needed.
- If you'd rather keep the repository private, GitHub Pages from a private repo requires a **GitHub Pro** account; on the free plan, the repo (and therefore the source code) must be public. The app's *data* is never uploaded anywhere, only the code that runs the calculator.
