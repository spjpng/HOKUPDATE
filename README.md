# HOUSE OF KINGS — Shopify Theme

A custom Shopify **Online Store 2.0** Liquid theme (silver & black, mobile-first, no paid apps).

## Stack & conventions

- **Type:** Shopify OS 2.0 theme (JSON templates + sections + section groups).
- **No build step.** Plain CSS (`assets/base.css`) + vanilla JS (`assets/theme.js`). No `package.json`, no Node, no SCSS.
- **Fonts:** Inter via Google Fonts (loaded in `layout/theme.liquid`). No font files in repo.
- **Images:** None bundled. All imagery comes from Shopify CDN (theme settings `image_picker`) or `placeholder_svg_tag` fallbacks.
- **Color/font tokens:** injected as CSS custom properties in `layout/theme.liquid` `<style>` from `settings.*`; consumed by `assets/base.css`.
- **Content:** all merchant content lives in `templates/*.json` and section/block settings — nothing hardcoded.

## Color & gradient editor

Every theme color flows from **Theme settings → Colors** into CSS variables. The "Gradients" group lets a merchant override any flat background (page, cards, footer, primary button, hero overlay, sections) with a gradient — leave blank to keep the solid color. Defaults reproduce the base look exactly.
