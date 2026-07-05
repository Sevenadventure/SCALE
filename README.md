# SCALE — Seattle Composers Alliance Logbook & Estimator

A finance logbook for working artists that lives in **one file** and keeps your data **on your device**. Import bank statements (PDF/CSV/paste), categorize with rules, forecast cashflow, estimate taxes, track hours and mileage, and generate invoices.

## Use it

- **Individuals, freelancers, small businesses:** https://sevenadventure.github.io/SCALE/for-individuals.html
- **Organizations** (program budgets, board reports, treasurer tools): https://sevenadventure.github.io/SCALE/for-orgs.html
- **Try a demo first:** [individual demo](https://sevenadventure.github.io/SCALE/for-individuals-demo.html) · [org demo](https://sevenadventure.github.io/SCALE/for-orgs-demo.html)
- **Download an offline copy:** grab the file from [Releases](../../releases/latest), then open it in your browser (double-click it). That is the whole install.

## Your data & privacy

- Everything is stored in your browser (localStorage). No accounts, no company server, no analytics, no tracking.
- The complete list of network activity: **(1)** importing a PDF downloads the open-source PDF reader ([pdf.js](https://mozilla.github.io/pdf.js/)) from the cdnjs CDN, and SCALE cryptographically verifies it before it runs; **(2)** any live sync you set up yourself talks only to your own Google Apps Script link. Nothing else touches the network.
- The online app and a downloaded copy keep **separate** data stores. Pick one home; move anytime with a Save & Restore backup file.
- This whole repository is the app. Anyone can read exactly what the code does.

## Verify a download

`SHA256SUMS.txt` lists checksums. After downloading:

```
shasum -a 256 <file>.html               # Mac
certutil -hashfile <file>.html SHA256   # Windows
```

Release notes also link a VirusTotal scan of each file.

## Backups

Save & Restore (in the app) downloads a single `.json` backup. Keep one somewhere safe; restoring it replaces what is in that browser.
