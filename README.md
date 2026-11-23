# Fasmie Hub – Retail Inventory & Sales Management System

A web app for running a phone case shop in Kenya. It replaces paper records and spreadsheets with one app that works on phone, tablet and desktop.

## Features

| Area | What it does |
|---|---|
| **Sell** | Tap a case photo to record a sale in seconds (iPhone, Samsung, accessories) |
| **Stock** | Monthly stock sheet per design and phone model: start, added, sold, left |
| **Restock** | Ranked shopping list of cases with 2 or fewer left, fastest sellers first |
| **Best sellers** | Top cases and phone models, slow movers, average selling price per case |
| **Sales channels** | Walk-in, TikTok Live, Jumia and Kilimall |
| **Dashboard** | Profit for today, this week or this month after cost of goods and bills |
| **Bills** | Rent, staff payments and other costs |
| **Designs** | Add a new case with a photo; it is numbered and appears everywhere at once |
| **Security** | Money figures hidden behind a password (SHA-256 hashed), re-locks after 10 minutes |
| **Backup** | One-click Excel export: summary, each month, bills, daily sales, designs |

Also: light and dark mode, mobile-first layout (bottom tabs on phones, sidebar on desktop).

## Tech

- HTML5, CSS (custom properties, grid, flexbox), vanilla JavaScript
- Cloud document database with live updates (`onSnapshot`)
- [SheetJS](https://sheetjs.com/) for Excel export
- Web Crypto API (SHA-256) for the password check
- Built with AI-assisted development (Claude)

## Running it

The app is one file, `index.html`. It saves its data through the Claude Artifacts runtime (`window.claude`), so it is meant to be opened as a Claude artifact. Opened as a plain web page it shows the layout but cannot save.

The demo password in this repository is `demo1234`. To set your own, replace `PASS_HASH` in `index.html` with the SHA-256 hash of your password.
