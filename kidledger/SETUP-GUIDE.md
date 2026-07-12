# Children's Expenses — setup guide

A dedicated app on your iPhone home screen. Everything is stored on the phone. Works offline. One-off setup of about ten minutes.

## Step 1 — Host the files (free, one-off)

1. Go to github.com and sign in (or create a free account).
2. Click New repository. Name it `expenses`, set it to Public, tick Add a README, and create it.
3. Click Add file → Upload files and upload all 7 files from this folder (the files, not the folder itself): index.html, sw.js, manifest.json, jspdf.umd.min.js, icon-180.png, icon-512.png.
4. Go to Settings → Pages. Under Source choose Deploy from a branch, branch main, folder / (root). Save.
5. After a minute or two your app is live at https://YOUR-USERNAME.github.io/expenses/

The public repository contains only the app code — no data and no keys. Your expenses and API key never leave your phone.

## Step 2 — Install on your iPhone

Open the address above in Safari → Share → Add to Home Screen → Add.

## Step 3 — Turn on automatic reading (optional)

Create an API key at console.anthropic.com (separate to a Claude subscription), add about £5 of credit, then in the app: gear icon → paste the key → Test key → Save settings. Roughly a penny per receipt.

## Using it

Everything starts from the Add expense button, six routes:

- Photograph receipt — single receipt, read automatically when online.
- Grocery receipt — camera or photo library; reads line by line, marks items children's / not / unsure. Tap the amber ? items in or out; included items set a fixed £ allocation.
- Bank statement — camera or photo library; pulls out payments, pre-ticks obvious child-related ones. Ticked items land in To review with the statement photo as evidence.
- Email receipt — paste the text of an emailed receipt (e.g. Tesco); items are classified like a grocery receipt and the text is kept as PDF evidence.
- Import photos — sweep in receipts snapped earlier; they land in To review for allocating later.
- Manual entry — no photo, type the details.

Tagging and allocating: every expense is tagged to a child or Both (splits 50/50 between the two bank accounts), given a category, and an allocation: 100%, 66%, 50%, 33%, a manual %, or a manual £ amount. The front page shows this month's total from each child's account.

Rules: tick "always use these settings for this merchant" when saving and future receipts from that merchant are pre-set automatically. Manage rules in Settings.

Exports: "PDF for accountant" on any month builds one evidence pack — summary table with per-child totals on page one, then every receipt (photo or email text) on its own page. Opens straight into the share sheet. A full-ledger CSV and tax-year summary (6 April to 5 April, per child) live in Settings.

Backup: Settings has one-tap backup (data plus photos) and restore. Download one occasionally to iCloud Drive or OneDrive — the data otherwise lives only on this phone.

Updating to a new version: upload the changed files over the old ones on GitHub, then fully close the app and reopen it twice.
