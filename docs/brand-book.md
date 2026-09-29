# Teebat Karbala

The design system of teebatkarbala.iq, the website of Teebat Karbala (طيبة كربلاء) and its flagship Karbala International Airport. Every token and component here is copied from the live site's stylesheet and computed styles (captured 29 September 2026), so new pages match what is already published. Tagline: "Iraq's Gateway to the World."

## Principles

- **Blue on white.** The site is white with one strong blue (`primary`, #1A76D1) that carries every action, the active nav, the stats band and the footer. `navy` is reserved for the info-card row, and `ink` is for headings and the dark button.
- **One family, Cairo.** Cairo sets Arabic and English alike. Headings are 600 (the hero headline 400), nav and buttons 500, body 400.
- **Soft motion.** Hovers ease over 0.3–0.4s: cards lift 5px, icon circles fill with `primary`, and the nav underline grows from the left. Nothing moves on its own.
- **Round icons, soft corners.** Icons sit in circles (`radius-round`). Buttons use `radius-4` and cards `radius-5`.

## Voice

Welcoming and proud, but formal: "Let's Connect! Whether you're a traveler, an airline or a partner…". Headings are capitalised ("Facts and Figures", "News And Updates"). Figures are big and plain ("40000 backfilling carried out"). Name the oversight body in full: the General Secretariat of The Husseiniya Shrine (العتبة الحسينية المقدسة).

## Colour

| Token | Value | Where on the site |
| --- | --- | --- |
| `primary` | #1a76d1 | Buttons, active/hover nav, links, footer and copyright, icon hovers, dotted connectors |
| `navy` | #0a4784 | Info cards under the hero |
| `ink` | #2c2d3f | Headings, nav at rest, top-bar links, "Learn More" button |
| `text-menu` | #666666 | Dropdown and mobile submenu links |
| `text` | #707070 | Body and secondary text, darkened from the site's greys to pass AA on every ground |
| `text-dark` | #333333 | Dark body copy |
| `surface` / `surface-alt` | #ffffff / #f8f8f8 | Page and alternate sections |
| `line` / `line-strong` | #eeeeee / #dddddd | Top-bar border / icon circle outlines |
| `field-border` | #8c8c8c | Form field outlines (darkened from the site's #eee) |
| `primary-overlay` | primary at 80% | Blue wash over photos (stats band) |

**Accessibility:** body text uses `text` (#707070: 5.0:1 on white, 4.7:1 on `surface-alt` and `surface-card`) instead of the site's lighter default #888 (3.5:1, which fails AA). White on `primary` is 4.6:1. The `line` greys are decorative only. Form fields are outlined in `field-border` (#8c8c8c, 3.4:1), not the site's near-invisible #eee.

`logo-blue` (#105989) and `logo-aqua` (#78c8d9) come from the company logo, and `sand` (#c09a60) from the airport logo. They are for logos and brand graphics, not UI.

## Type

All type is Cairo, loaded from Google Fonts (the site self-hosts `Cairo-Regular`). The styles:

- `hero` 38/42, weight 400; `hero-subtitle` 20/24, weight 500
- `section-title` 32/38.4
- `stat` 30
- `feature-title` 21
- `card-title` 20
- `news-title` 24, weight 500
- `lead` 19
- `body` 18/24
- `nav` 18, weight 500
- `small` 15
- `button` and `topbar` 14

In the hero, the key word ("Karbala") is set in `primary` at weight 400 inside an `ink` headline.

## Layout

Sections are padded `space-120` top and bottom, and the footer's top band `space-100`. Cards are padded `space-30` and buttons 13px × `space-25`. Content sits in a centred Bootstrap container, 1140px at its widest. Home page order: header, hero with photo, info-card row, section title, features row, stats band over a photo, news, footer.

## Components

These are CSS classes in `components/bundle.css` (prefix `tk-`), built on the tokens. Each has a live preview and guidelines, and most previews show English and Arabic side by side.

- **Navigation:** Header, Dropdown, MobileMenu, Footer
- **Content:** Hero, SectionTitle, InfoCard, Feature, StatsBand, NewsCard, PartnerStrip
- **Actions and forms:** Button, FormField

Values are measured from the live site, apart from the form states (which the site lacks) and the darker form-field outline. Where the site has a flaw (the tiny phone headline, the news tag's off-brand blue, the small mobile menu button), the component's guidelines flag it and say what to do instead.

## Arabic

The site has a full Arabic version at `/ar/` (`lang="ar" dir="rtl"`), set in the same Cairo family. Wrap Arabic pages or blocks in `dir="rtl" lang="ar"`, and every component mirrors:

- the nav underline grows from the right;
- the feature connectors run right to left;
- the hero text sits on the right.

Arabic headings are never capitalised or letter-spaced. Arabic needs taller line spacing, so use the `ar-*` type styles (line height about 1.5, against 1.2–1.3 for English). Keep numerals consistent within a page: the site uses Western digits (40,000, 64) in both languages. In the header, the language switch reads "اللغة العربية" on English pages and "English" on Arabic ones.

## Iconography

Icons come from IcoFont, as on the site: single-colour glyphs that take the surrounding text colour. The ones in use are in the Icons asset group.

- **Outlined circle:** in features, a 50px `primary` icon inside a 100px circle outlined in `line-strong`, which fills with `primary` on hover.
- **Stats band:** 28px white icons in 70px white-ringed circles.
- **Footer:** social icons in 34px white-ringed circles.

IcoFont is licensed CC BY 4.0, so credit it on the site.

## Logos

- **Company logo** (`assets/Logos/teebat_karbala_company_logo.png`): an eight-point star in `logo-blue` (#105989) and `logo-aqua` (#78c8d9), with طيبة كربلاء above "Teebat Karbala". It is the primary mark, used at the left of the header, about 48px tall. The PNG is 4000px wide with a transparent background.
- **Airport logo:** use `kia_logo_large.jpg` (2048px) on light grounds and `kia_logo_reversed.jpg` (white and gold on navy, 2048px) on dark ones. Both come from the airport project's Facebook page. The original `kia_logo.jpg` is only 200px. Use the airport logo for airport-specific material only.

Use the full-colour logos as supplied, on white, with at least `space-30` clear space. Never recolour, stretch or redraw them. `logo-blue`, `logo-aqua` and `sand` are logo colours, not UI colours.

Still needed: SVG versions of both logos, a standalone reversed company logo, and the star mark on its own.

## Imagery

Use real project photography: engineers and workers on site, the terminal's steel and façade, and aircraft once operations start. The Photography asset group holds four site photos from the airport project's Facebook page. Photo bands take the `primary-overlay` wash with white text on top. Partner logos (the Holy Shrine, ADP and others) appear on a white strip. No stock images or AI renders.
