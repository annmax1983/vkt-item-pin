# VKT Item Pin

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A shopping research extension that captures product snapshots with one hover: title, price, link, model, site and date are saved to a local library, with automatic price-history tracking.

> Chromium-based · Manifest V3 · Minimal Permissions · No Tracking · 100% Local

---

## Why VKT Item Pin?

Comparing products across shopping sites usually means dozens of open tabs and copy-pasting into spreadsheets. VKT Item Pin lets you hover any product, click **Pin**, and keep a growing price-tracked library — right in your browser.

| Advantage | Detail |
|-----------|--------|
| 🎯 **Hover to Capture** | Hover a product, click the Pin button — title, price, link, model, site and date are extracted automatically |
| 📈 **Price History** | Re-capture the same product any time — each visit appends a new price point and builds a trend chart |
| 🛒 **24 Site Presets** | Hand-tuned selectors for Amazon, eBay, Etsy, Walmart, AliExpress, Temu and more — plus a universal engine (JSON-LD / OG / generic selectors) for every other shop |
| 🖼️ **Thumbnails** | Product images are saved with each record |
| 🔒 **Privacy First** | All data stays in your browser via `chrome.storage.local`. Nothing is uploaded |

---

## Features

### 🆓 Free

| Feature | Description |
|---------|-------------|
| 🎯 **One-Click Capture** | Hover any product on product pages or listing/search pages and pin it |
| 📋 **Preview & Pick** | Edit fields before saving; "Pick" mode lets you click any element on the page to fill a field |
| 📈 **Price History** | Unlimited re-captures on tracked products — each capture adds a price point, with a trend chart per item |
| ✏️ **Edit Records** | Fix titles/models, correct or remove bad price points |
| 💾 **JSON Backup** | Export / import a full backup of your library (works offline) |
| 🧮 **Storage Monitor** | Shows real storage usage and warns before it gets full |
| 🌍 **6 Languages** | English, Chinese, Japanese, Spanish, German, French |

### ⭐ Pro (License Required)

| Feature | Description |
|---------|-------------|
| ♾️ **Unlimited Products** | Free plan covers 50 products; Pro removes the limit |
| 🔍 **Advanced Filters** | Filter by site, date range and price range |
| 📤 **CSV Export** | Export your library (with BOM, Excel-friendly) |
| 📊 **Multi-Item Compare** | Overlay price history of up to 6 products in one chart |

---

## Supported Sites

**Hand-tuned presets (24):** Amazon (all marketplaces), eBay, Etsy, Walmart, Target, AliExpress, Temu, Best Buy, Home Depot, Lowe's, Newegg, Wayfair, Mercari, Shopee, Lazada, Rakuten, SHEIN, Alibaba.com / 1688, DHgate, TikTok Shop, bol.com, Allegro, Otto.de, Cdiscount …

**Everything else** (Shopify / WooCommerce / independent shops) is covered by the universal engine: JSON-LD structured data → Open Graph tags → generic selectors → regex fallback → manual pick mode.

---

## Supported Browsers

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Fully supported |
| Microsoft Edge | ✅ Fully supported |
| Other Chromium-based browsers | ✅ Should work |

---

## Installation

1. Open your browser's extension page:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
2. Enable **Developer mode** (top-right toggle)
3. Click **Load unpacked** and select the `vkt-item-pin` folder
4. Hover any product on a shopping page and click the 📌 Pin button

---

## Usage

### Capture a Product

1. Hover any product (on a detail page **or** in a search-result grid) — a 📌 button appears
2. Click it — a side panel opens with the extracted title, price, link, model, site and date
3. Correct anything, use **Pick** to grab a missing field, then click **Save**

### Track Prices

- Re-capture a product you already saved — a new price point is appended automatically (tracked products never count against the free limit)
- Open the dashboard to see the trend chart, or use **Compare** (Pro) to overlay multiple products

### Backup

- The dashboard footer has **Backup JSON** / **Import** for full-library backups — recommended regularly, since data lives only in your browser

---

## How It Works

```
Hover a product → click Pin
       ↓
Extractors run (JSON-LD → site preset → generic → regex)
       ↓
Preview panel: edit / pick fields
       ↓
Saved to chrome.storage.local (URL normalized & de-duplicated)
       ↓
Re-capture appends a price point → trend chart in dashboard
```

All extraction and storage happen locally in your browser. The only network request is **optional** — when you activate a Pro license key, the extension contacts the license server with your key and basic browser metadata (browser, language, timezone). No webpage content is ever read or uploaded.

---

## Privacy

- `storage` — Saves your product library locally. No webpage content leaves your browser.
- `scripting` + `activeTab` — Inject the Pin button / extract fields only while you interact with the page.
- `<all_urls>` — Lets the extension work on every shopping site. It never reads or uploads page content in the background.
- No tracking, no analytics. The only network request is license activation/validation when you use a Pro license key.

---

## License

Copyright © 2026 VKT Item Pin. All rights reserved.

---

## ❤️ Support

If you find VKT Item Pin helpful, consider supporting the project!

**[👉 Get a License Key](https://www.annmax1983.com/checkout.html?plugin=itempin)** · [GitHub](https://github.com/annmax1983/ItemPin) · [Official Website](https://www.annmax1983.com/extensions/itempin)
