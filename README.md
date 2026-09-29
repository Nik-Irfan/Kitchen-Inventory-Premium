# My Kitchen

[React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
[TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?logo=typescript&logoColor=white)
[Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-06B6D4?logo=tailwindcss&logoColor=white)
[Vite](https://img.shields.io/badge/Vite-5.0-646CFF?logo=vite&logoColor=white)
[License](https://img.shields.io/badge/License-MIT-green)

> Minimal, premium pantry tracker with batch expiry, low-stock alerts, and smart shopping — 100% local, no backend.

**Live Demo:** https://nik-irfan.github.io/Kitchen-Inventory-Premium/

---

### Overview

My Kitchen helps you track what you actually have. Each item supports multiple batches (e.g., 2x Basil bought on different dates), optional expiry tracking, and automatic shopping list generation when stock is low or expiring.

Built mobile-first. All data stays on your device in localStorage — no account, no cloud.

---

### Features

| Area | What it does |
|------|--------------|
| **Kitchen** | Batch-based inventory, expiry ON/OFF per item, low-at threshold, status dots (Good / Low / Expiring ≤3d / Expired) |
| **Search** | Sticky liquid-glass header, filters by category & status |
| **Shopping** | Auto-populates low/expiring/expired items, Select all / Deselect all, qty-to-buy modal |
| **Pagination** | Clean 3-button `All | 10 | 20` — customizable in Settings → System, single glass pill, compact + comfortable |
| **Cards** | Compact 68px & Comfortable 110px, ✎ edit, checkbox animation, qty control |
| **Share** | WhatsApp primary + system share fallback, Buy selected merges into inventory |
| **Settings** | Single-open accordions — Appearance (8 themes), Categories, Units, System, Data |
| **Data** | Save as .txt, Add list paste, 100% local storage |

---

### Tech Stack

- **Framework:** React 18 + TypeScript
- **Styling:** Tailwind CSS, custom keyframes, liquid glass `blur(24px) saturate(180%)`
- **Fonts:** Fraunces (serif) + Inter (sans)
- **State:** React `useState` + `useMemo`, localStorage
- **Build:** Vite-ready — single `App.tsx`, no extra dependencies

---

### Quick Start

```bash
git clone https://github.com/nik-irfan/Kitchen-Inventory-Premium.git
cd Kitchen-Inventory-Premium
npm install
npm run dev
```

Open `http://localhost:5173`

---

### Usage

1. **Add item:** Tap `+` FAB → Name, Unit, Category, Low-at, Use by date toggle
2. **Batch entries:** Edit item → Entries (Latest on top) → Add/edit qty + expiry
3. **Quick qty:** Use `- +` on kitchen cards
4. **Shopping:** Check items → Set buy qty → Share or Buy selected
5. **Customize:** Settings → System → First size / Second size (5-100)

All data is stored locally: `mykitchen-items`, `mykitchen-categories`, `mykitchen-units`, `mykitchen-theme`, `mykitchen-perpage-options`, `mykitchen-perpage`

---

### Project Structure

```
src/
  App.tsx
  index.css
  main.tsx
```

---

### Customization

**Themes (8)** — Paper, Sage, Clay, Ink, Oat, Matcha, Midnight, Terracotta

**Pagination** — Settings → System → First size (10) / Second size (20). UI stays `All | {opt1} | {opt2}` — single glass pill `w-fit`.

---

### License

MIT — free to use, keep attribution.
