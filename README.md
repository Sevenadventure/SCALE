# SCALE — Seattle Composers Alliance Logbook & Estimator

A personal-finance logbook for individuals and small businesses that lives in **one file** and keeps your data **on your device**. Import bank statements (PDF/CSV/paste), categorize with rules, forecast your cashflow, estimate taxes, track hours, and generate invoices.

## Use it

- **Open the app:** https://YOUR-USERNAME.github.io/scale/  *(starts blank; your data stays in your own browser)*
- **Try the demo first:** https://YOUR-USERNAME.github.io/scale/demo.html  *(pre-filled with fictional data, safe to experiment with)*
- **Download an offline copy:** grab the `.html` from the [Releases](../../releases) page and open it in any browser. That is the entire install.

For organizations (program budgets, board reports, treasurer check-request tools for fiscally sponsored orgs): [org.html](https://YOUR-USERNAME.github.io/scale/org.html) · [org demo](https://YOUR-USERNAME.github.io/scale/org-demo.html)

## Your data & privacy

- Everything is stored in your browser (localStorage). No accounts, no company server, no analytics, no tracking.
- The complete list of network activity: **(1)** importing a PDF downloads the open-source PDF reader ([pdf.js](https://mozilla.github.io/pdf.js/)) from the cdnjs CDN, and SCALE cryptographically verifies it before it runs; **(2)** any live sync you set up yourself talks only to your own Google Apps Script link. Nothing else touches the network.
- The online app and a downloaded copy keep **separate** data stores. Pick one home; you can move anytime with a Save & Restore backup file.
- This whole repository is the app. Anyone can read exactly what the code does.

## Verify a download

Each release lists SHA-256 checksums (`SHA256SUMS.txt`). After downloading:

```
shasum -a 256 <file>.html     # Mac
certutil -hashfile <file>.html SHA256   # Windows
```

Compare against the published value. Release notes also link a VirusTotal scan of each file.

## Backups

Save & Restore (in the app) downloads a single `.json` backup. Keep one somewhere safe; restoring it replaces what is in that browser.
