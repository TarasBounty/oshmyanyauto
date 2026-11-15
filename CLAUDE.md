# CLAUDE.md — rules for working on this repo

## Project

One-page website for **Автохаус «Ошмяны Авто»** (car dealership in Ошмяны, Belarus).
Services: кредит, лизинг, обмен, срочный выкуп, ваш авто в зачёт (trade-in), помощь в продаже.

## Business facts (single source of truth — do not invent others)

- Name: Автохаус «Ошмяны Авто» (logo: АВТО + ХАУС in gold, subtitle «ОШМЯНЫ АВТО»)
- Address: г. Ошмяны, ул. Пионерская, 60А — Yandex Maps: https://yandex.ru/maps/-/CXvneB5a
- Phone: +375 (29) 307-34-43 (`tel:+375293073443`)
- Telegram: https://t.me/oshmyanyauto
- Instagram: https://www.instagram.com/oshmyanyauto (cars in stock are published there)
- Hours: ежедневно, без выходных, 9:00–20:00
- УНП 591716034

Never add prices, interest rates, bank names, terms or other claims that are not listed here.
If a change needs new facts, ask for them or leave a clearly marked `TODO` placeholder.

## Tech

- Plain static site: `index.html`, `assets/css/style.css`, `assets/js/main.js`, `assets/img/`.
- No build step, no frameworks, no npm. Files are deployed as-is (GitHub Pages / Hostinger `public_html`).
- Use relative paths only (the site may be served from a sub-path on GitHub Pages).
- Language of all site content: Russian.
- External resources allowed: Google Fonts (Montserrat), Yandex Maps widget. Nothing else (no trackers) unless asked.

## Design

- Dark charcoal background (`--bg`) with a faint repeating car pattern, gold gradient accents (`--gold`).
- Headings: Montserrat 900, italic, uppercase. Body: Montserrat 400–600.
- Reuse the CSS variables and existing components (`.btn--gold`, `.btn--outline`, `.card`, `.section__title`).
- Mobile-first quality: check at 375px width — no horizontal scroll, tap targets ≥ 44px.

## Workflow

- Every change goes through a pull request into `main`; never push to `main` directly.
- One logical change per PR, with a short description of what changed and how to check it.
- Before opening a PR, render the page at desktop (1440px) and mobile (375px) widths and check it visually.
