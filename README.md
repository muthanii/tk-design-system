# Teebat Karbala Design System

The design system for [teebatkarbala.iq](https://teebatkarbala.iq), the website of Teebat Karbala (طيبة كربلاء) and the Karbala International Airport project. Colours, type, spacing and components are measured from the live site, with a few accessibility fixes noted in the brand book.

**Internal use only.** The logos, photos and brand belong to Teebat Karbala Company. Keep this repository private.

## What's here

| Path | What |
| --- | --- |
| `tokens.json` | All design tokens (colours, type styles, spacing, radii, shadows) with usage notes |
| `tokens.css` | The same tokens as CSS custom properties (`--primary`, `--space-30`, …) plus one class per type style |
| `components/components.css` | Component styles, prefixed `tk-` (buttons, header, hero, cards, forms, footer, mobile menu), with right-to-left support |
| `components/*.html` | A live preview page for each component. Open `index.html` to browse them |
| `docs/brand-book.md` | The brand book: principles, voice, colour, type, layout, Arabic, iconography, logos, imagery |
| `docs/components/*.md` | Usage guidelines for each component |
| `assets/logos/` | Company logo (PNG) and airport logos (full size, reversed, original) |
| `assets/photography/` | Project site photos |
| `assets/icons/` | The IcoFont icons the site uses, as SVG |

## Using it on a page

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700&display=swap">
<link rel="stylesheet" href="tokens.css">
<link rel="stylesheet" href="components/components.css">

<body class="tk">
  <a class="tk-btn" href="/contact.html">Contact us</a>
</body>
```

For Arabic pages, add `dir="rtl" lang="ar"` to `<html>`; the components mirror automatically.

## Credits

- Icons: [IcoFont](https://icofont.com), licensed CC BY 4.0. Credit "Icons by IcoFont" on the site.
- Typeface: [Cairo](https://fonts.google.com/specimen/Cairo), SIL Open Font License.
- Airport logos and photos: Karbala International Airport Project ([facebook.com/KIA.PROJECT](https://www.facebook.com/KIA.PROJECT/)).

## Still missing

- SVG versions of the company and airport logos
- A standalone white (reversed) company logo, and the star mark on its own for favicons
- Larger original photos for full-width hero images
