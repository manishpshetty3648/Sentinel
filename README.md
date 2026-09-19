# 🛡️ Sentinel

### Silent-Loss Intelligence for Small Business

*Stop losing money you can't see.*

Built by team **NxtOps** for the Bharat Builds Tour · First Commit hackathon.

## The Problem

Small businesses rarely lose money in one big mistake. They lose small amounts, repeatedly, through problems they never notice: dead stock, stockouts, degrading suppliers, creeping prices, high return rates and overdue payments.

## The Solution

Sentinel scans a shop's operational data (products, sales, purchase orders, returns, invoices), detects silent losses, and explains the root cause behind each one.

## Features

- Multiple detectors across inventory, suppliers, returns, pricing and receivables
- "Explain Why" evidence trail on every finding
- Unmet-demand estimation during stockouts
- Add / edit / delete your own data with live re-scan
- Built-in AI assistant for questions about your data
- Liquid-glass UI with dark and light themes, responsive on all devices

## Run locally

Sentinel is a single static file. No build step needed.

```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

## Deploy on AWS Amplify Hosting

1. Push this repo to GitHub.
2. Open the AWS Console → **AWS Amplify** → **Create new app** → **Host web app**.
3. Choose **GitHub**, authorize, and select this repository and the `main` branch.
4. Amplify detects `amplify.yml`. Leave the defaults and click **Save and deploy**.
5. When the build finishes, open the generated `https://main.<app-id>.amplifyapp.com` URL.

Every `git push` to `main` redeploys automatically.

## Project structure

```
sentinel/
├── index.html    # the complete app (HTML + CSS + JS)
├── amplify.yml   # Amplify build settings (static site, no build)
├── README.md
├── LICENSE
└── .gitignore
```

## Team

NxtOps: Nandu Reddy, Dhruva Reddy J, Ankith G Prasad, Manish P Shetty

## License

MIT, see [LICENSE](LICENSE).
