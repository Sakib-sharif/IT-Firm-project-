# IT Hub — IT Services Website

A multi-page static website for a fictional IT services firm called **IT Hub**. Built with vanilla HTML, CSS, and JavaScript — no build step, no framework, no dependencies (one Google Fonts link).

## What's in the box

```
it-hub/
├── index.html              ← Home page
├── services.html           ← All 9 services, long-form
├── pricing.html            ← 3 tiers + comparison table + FAQ
├── industries.html         ← 7 industry cards
├── case-studies.html       ← 6 customer stories
├── resources.html          ← Blog + help center + status + events
├── about.html              ← Story + values + team + careers + partners
├── contact.html            ← Contact form + offices
├── signin.html             ← Customer portal sign-in
├── privacy.html            ← Privacy policy template
├── terms.html              ← Terms of service template
├── assets/
│   └── styles.css          ← Shared stylesheet
└── README.md               ← This file
```

## Quick start — Option A (easiest)

Just open it in your browser:

1. **Unzip** the archive
2. **Double-click** `index.html`
3. It'll open in your default browser. Done.

> ⚠️ Some browsers restrict certain features on `file://` URLs (like Google Fonts loading). If anything looks off, use Option B.

## Quick start — Option B (recommended, takes 10 seconds)

Serve it with any local HTTP server. Pick whichever you have installed:

### If you have Python 3 (most macOS/Linux come with it):
```bash
cd it-hub
python3 -m http.server 8000
```
Then open **http://localhost:8000** in your browser.

### If you have Node.js:
```bash
cd it-hub
npx serve .
# or
npx http-server -p 8000
```
Then open **http://localhost:8000**.

### If you have PHP:
```bash
cd it-hub
php -S localhost:8000
```

### If you have Ruby:
```bash
cd it-hub
ruby -run -e httpd . -p 8000
```

## Deploying to the web

It's pure static — drop it on any static host:

| Host | How |
|---|---|
| **Netlify** | Drag-and-drop the `it-hub` folder at https://app.netlify.com/drop |
| **Vercel** | `npx vercel` inside the `it-hub` folder |
| **GitHub Pages** | Push to a repo, enable Pages in repo settings |
| **Cloudflare Pages** | Connect the repo or upload the folder |
| **AWS S3** | Upload the folder contents to a public bucket |
| **Any web host** | Upload via FTP/SFTP to your `public_html` (or equivalent) |

## Customizing

All copy and branding is plain HTML — open any `.html` file in a text editor and edit directly. Common changes:

| What | Where |
|---|---|
| Brand name | Search & replace `IT Hub` in all `.html` files |
| Logo mark | Edit `.logo-mark` in `assets/styles.css` |
| Accent color | Change `--accent` and `--grad-1` in `assets/styles.css` `:root` |
| Service descriptions | `services.html` |
| Pricing tiers & prices | `pricing.html` |
| Case studies | `case-studies.html` |
| Office locations | `contact.html` (search for "San Francisco") |
| 24/7 phone number | Search for `1-800-IT-HUB-1` in all `.html` files |
| Email addresses | Search for `@ithub.com` in all `.html` files |
| Compliance badges | Search for `SOC 2 Type II` in all `.html` files |

> 💡 **Tip:** For multi-file search-and-replace, VS Code, Sublime, or `sed -i ''` (macOS) / `sed -i` (Linux) all work great.

## Browser support

Tested on the latest Chrome, Safari, Firefox, and Edge. Uses modern CSS (Grid, custom properties, `clamp()`, `backdrop-filter`) and IntersectionObserver — works on any browser from 2020+.

## What this is *not*

- ❌ Not a CMS — edit files directly
- ❌ Not a framework — vanilla HTML, no React/Vue/etc.
- ❌ Not connected to a backend — forms don't actually submit anywhere
- ❌ Privacy & Terms pages are **template placeholders** — have a lawyer review before going live

## License

Use it, change it, ship it. No attribution required.
