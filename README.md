# Royal Agar Attar: B2B website (new)

Second, English-first site for foreign wholesale buyers. Single static page, no build step.

- `index.html`: the whole page. Styles in one `<style>` block, scripts in one `<script type="module">` block.
- `assets/js/lenis.mjs`: smooth scroll (self-hosted).
- `assets/img/`: images from the main site. Most bottle images are AI renders; replace them with real photos.
- `assets/video/`: real process footage, one clip per step of the "From tree to oil" film.
- Fonts: Cormorant Garamond (headings) and Onest (body) from Google Fonts.

## Brand palette

| Token | Hex | Use |
|---|---|---|
| Parchment | `#f4efe6` | page background |
| Resin | `#17110c` | dark cards, hero, footer |
| Gold | `#c9a46a` | accents on dark only (fails contrast on parchment) |
| Bronze | `#7a5a1a` | gold-toned text on light |
| Maroon | `#6e1e2e` | accent instead of green |

## Claim rules (keep these when editing copy)

- No "pure", "100% pure", "certified", "lab tested" or "organic" until there is a lab report.
- No shipping or export claims until CITES export permits are in place.
- Wood is bought from growers and suppliers; do not say "we grow our own trees".
- Say "nothing added after distillation".

## Tracking

The page pushes `whatsapp_click`, `quote_open` and `generate_lead` to `dataLayer`. Paste a GTM ID in the marked block in `index.html` to send them to GA4 / Meta.

## Hosting

Static files. `netlify.toml` publishes the repo root. Works the same on any free static host (Netlify, Cloudflare Pages, GitHub Pages, Vercel).
