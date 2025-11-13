# WhatsApp Game Day – Formatter (v1.0)

A tiny, single-file web app that turns raw game notes into a polished WhatsApp announcement with the correct order, emojis, and formatting rules. Runs 100% client-side (privacy-friendly), works great on mobile, and includes one-tap **Copy**, **Share**, and **Open in WhatsApp** actions.

---

## ✨ Features

- Instant preview with seeded example message; updates as you type
- Strict field order and emoji layout for Game Day posts
- Smart formatting rules
  - Title-case for all fields  
  - **Arrival**: only the first character capitalized (unless you type CAPS)
  - **FC** forced to uppercase (works even if typed as `fc`)
  - Preserves **ALL-CAPS** inputs (e.g., JCL, MVFC)
  - Time normalization → `h:mm am/pm` (lowercase, space) when meridiem is present
- One-tap actions: Copy text, Web Share API, or open WhatsApp (wa.me link)
- Mobile-first UI, works offline (no backend)
- Privacy: No analytics, no tracking, no network calls

## 🚀 Quick Start (Local)

1. Download this repository.
2. Open `index.html` in your browser.
3. Type into any field under “Fill in details”; the WhatsApp preview updates line-by-line.
4. Use **Copy**, **Share…**, or **Open in WhatsApp**.

> **iPhone note:** Clipboard is most reliable over HTTPS (GitHub Pages / Netlify). For a local file, long-press the preview → Select All → Copy.

## 🌐 Deploy to GitHub Pages (preconfigured)

This repo includes a **GitHub Pages** workflow.

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **GitHub Actions**.
4. The provided workflow will publish automatically.
5. Your site will be available at `https://<user>.github.io/<repo>/`.

## 🧠 Formatting Rules

- Order: Title → Teams → Date → Location → Warm-up → Kick-off → Kit → Snacks/Fruit → Arrival
- Title-casing for all fields, except Arrival (first character only)
- Preserve ALL CAPS fields (e.g., MVFC)
- Force “FC” uppercase regardless of input case
- Time format: `h:mm am/pm` if meridiem is present; otherwise `h:mm`

## 🧪 Versioning
- **v1.0** — stable

License: MIT (or your preference).
