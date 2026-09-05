# Duty & Interest Ledger

A single-page, browser-based ledger for tracking monthly dues, arrears, interest, and payments. No backend, no build step, no database — it's one self-contained HTML file that runs entirely in the browser.

**Live app:** _(add your GitHub Pages link here once deployed, e.g. `https://YOUR-USERNAME.github.io/duty-interest-ledger/`)_

## How it works

- All calculations happen client-side in JavaScript.
- Your data is **not** sent to any server. Nothing is stored remotely.
- Use the **Save Ledger** button (in the settings drawer) to download your data as a `.json` file, and **Import Saved Ledger** to reload it later. Save regularly — closing the tab without saving loses unsaved changes.
- The **Complete Report** tab can be turned into a PDF using its **Save as PDF** button (uses your browser's print dialog).

## Deploying to GitHub Pages (free hosting)

You only need a GitHub account. No coding required — just uploading a file.

### Step 1 — Create a new repository
1. Go to [github.com](https://github.com) and log in (or create a free account).
2. Click the **+** icon (top right) → **New repository**.
3. Name it something like `duty-interest-ledger`.
4. Set it to **Public** (required for free GitHub Pages hosting).
5. Click **Create repository**.

### Step 2 — Upload the files
1. On your new repository's page, click **Add file** → **Upload files**.
2. Drag and drop (or select) these two files:
   - `index.html`
   - `README.md`
3. Scroll down and click **Commit changes**.

### Step 3 — Turn on GitHub Pages
1. In your repository, go to **Settings** (top menu).
2. In the left sidebar, click **Pages**.
3. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
4. Under **Branch**, select **main** and folder **/ (root)**, then click **Save**.
5. Wait 1–2 minutes. Refresh the page — GitHub will show a green banner with your live URL, in the form:
   ```
   https://YOUR-USERNAME.github.io/duty-interest-ledger/
   ```

### Step 4 — Visit your site
Open that URL in any browser. The ledger app will load and work exactly as it does locally — anyone with the link can use it, and each visitor's data stays private to their own browser.

## Updating the app later

If you make changes to `index.html`:
1. Go to the file in your GitHub repository and click the pencil (✏️) **Edit** icon, or use **Add file → Upload files** to replace it.
2. Commit the change.
3. GitHub Pages will automatically redeploy within a minute or two — no extra steps needed.

## Notes

- The file loads one external script (SheetJS, for Excel export) from a public CDN (`cdnjs.cloudflare.com`). No API keys or accounts are required for this.
- Because everything runs client-side, GitHub Pages' free static hosting is sufficient — no server, database, or paid plan needed.
- If you'd rather keep the repository private, GitHub Pages from a private repo requires a **GitHub Pro** account; on the free plan, the repo (and therefore the source code) must be public. The app's *data* is never uploaded anywhere, only the code that runs the calculator.
