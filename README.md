# Gulgulii

Decoration Company

Website for GulGulii (گلگلی): flowerwork, handcrafts, gift packaging, wedding stage design, bride and groom bedroom decoration and wedding car flowers in Kabul.

- Live site: https://alphadudesnft-coder.github.io/Gulgulii/
- Plain static site with no build step: `index.html`, images in `img/`, self-hosted fonts in `fonts/`.
- Publishing: GitHub Pages, Settings > Pages > Build and deployment > Deploy from a branch > `main` / `(root)`. Every push to `main` goes live a minute or two later. Leave "Custom domain" empty unless a domain has been bought.

## Editing

- Languages: Dari (default, right to left) and English, switched with the button in the header. Text for both languages lives in the `T` object near the bottom of `index.html`. The Dari text written in the HTML is only the starting copy; `T` overwrites it on load, so change both.
- Prices and service descriptions live in the `SERVICES` list. The two price lists in the HTML (`#list-wedding`, `#list-crafts`) hold a pre-filled Dari copy for visitors without JavaScript; refresh it after changing prices.
- Business details that appear outside `T`:
  - WhatsApp number: the `WA` constant, the visible number in `#contact`, and the plain `https://wa.me/...` links.
  - Poolam wallet: the `#wallet-num` text (the Copy button copies whatever is shown there).
  - Instagram and Facebook links: `#gallery` and `#contact`.
  - Page titles: `<title>` and `document.title` in `render()`.
  - Search and link-preview text: the `description` and `og:` tags in `<head>`.
