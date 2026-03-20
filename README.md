# 📈 AI Stock Analyst Terminal

> Institutional-quality equity research reports for any stock ticker — powered by Claude AI with live web search.

![Static Badge](https://img.shields.io/badge/Powered%20by-Claude%20AI-00e5a0?style=flat-square)
![Static Badge](https://img.shields.io/badge/Deployed%20on-GitHub%20Pages-blue?style=flat-square)
![Static Badge](https://img.shields.io/badge/License-MIT-gray?style=flat-square)

---

## What It Does

Paste any stock ticker and get a structured, analyst-style research report in seconds. The AI pulls live news, earnings data, and market sentiment from the web to generate a report covering:

- **Company Overview** — business model, sector, market cap
- **Recent Developments** — latest earnings, news, and strategic moves
- **Financial Snapshot** — revenue growth, margins, valuation multiples
- **Bull Case** — the strongest reasons to be long
- **Bear Case** — genuine risks and headwinds
- **Technical Picture** — price trend and key levels
- **Analyst Consensus** — Wall Street buy/hold/sell distribution and price targets
- **Verdict** — an overall risk/reward assessment

## Demo

![Terminal screenshot placeholder](https://via.placeholder.com/900x500/080c0e/00e5a0?text=AI+Stock+Analyst+Terminal)

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/stock-analyst.git
cd stock-analyst
```

### 2. Get an Anthropic API key

Sign up at [console.anthropic.com](https://console.anthropic.com/settings/keys) and create a new API key. It starts with `sk-ant-...`.

### 3. Open the app

Just open `index.html` in your browser — no build step, no dependencies.

```bash
open index.html
```

### 4. Enter your API key

Paste your `sk-ant-...` key into the banner at the top of the page and hit **SAVE KEY**. It's stored in `localStorage` so you only need to do this once per browser.

## Deployment

This is a zero-dependency single HTML file. Deploy it anywhere static files are served.

### GitHub Pages

1. Push `index.html` to a public repo
2. Go to **Settings → Pages**
3. Set branch to `main`, folder to `/ (root)`
4. Your site will be live at `https://your-username.github.io/stock-analyst/`

### Other options

| Platform | Command |
|---|---|
| Netlify | Drag & drop `index.html` at [netlify.com/drop](https://netlify.com/drop) |
| Vercel | `vercel --prod` in the project folder |

## Tech Stack

| Layer | Tech |
|---|---|
| AI Model | Claude Sonnet (Anthropic) |
| Data | Anthropic Web Search tool |
| Frontend | Vanilla HTML / CSS / JS |
| Fonts | IBM Plex Mono + IBM Plex Sans |
| Hosting | GitHub Pages |

## Security Note

Your API key is stored in your browser's `localStorage` and is only ever sent directly to `api.anthropic.com`. It is never logged or transmitted anywhere else. That said, **do not share your deployed URL publicly** if you have your key saved in the browser — anyone with access to that browser session could extract it.

For a public-facing deployment, consider wrapping the API call in a serverless backend function that holds the key server-side.

## License

MIT — do whatever you want with it.

---

*Not financial advice. This tool is for informational and educational purposes only. Always consult a licensed financial advisor before making investment decisions.*
