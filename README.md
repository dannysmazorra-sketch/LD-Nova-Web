# LD Nova website (static, GitHub Pages ready)

```
index.html · css/styles.css · js/main.js · js/translations.js · assets/images/
```

## Images (assets/images/)
- `ld-nova-logo.jpg`, `logo-mark.png`, `favicon.png` — already included (from your logo).
- `founder-1.jpg` → Ledian RaIdel Reina Yanqui · `founder-2.jpg` → Dannys De Jesus Mazorra Rua (portrait, ~4:5).
- `promo-1.jpg` (hero + showcase), `promo-2.jpg`, `promo-3.jpg` — the three promotional images.
Until a file exists, the page shows a clean placeholder (hero falls back to the logo).

## WhatsApp
In `js/main.js` edit `CONFIG.waNumber` (digits only, country code included, e.g. `971553767656`).
Set `waVerified: false` to disable every WhatsApp button and the floating button until confirmed.
Prefilled messages (EN/ES) are `wa_msg` in `js/translations.js`.

## Email, pricing, founders
- Email: `CONFIG.email` in `js/main.js` and the visible address in `index.html` (search `solution@powerldai.tech`).
- Pricing: section `#pricing` in `index.html` (and the matching `r2`–`r13`, `q5` entries in `js/translations.js`).
- Founders: section `#founders` in `index.html` (titles/bios are placeholders `u3`, `u4`).

## Translations
English text lives in `index.html`; Spanish in `window.ES` in `js/translations.js`. Keys match `data-i18n`. The choice is saved in the browser.

## Contact form
Without a backend the form validates and opens the visitor's email app (mailto). For a real form service (Formspree, Getform…) paste its URL in `CONFIG.formEndpoint`. Never put private API keys in this code.

## Publish on GitHub Pages
Create a repository, upload all files (keep the folder structure), then Settings → Pages → Deploy from branch → `main` / root. Set `CONFIG.siteUrl` to the final URL for the canonical link.
