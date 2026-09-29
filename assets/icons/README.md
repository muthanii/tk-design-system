# Icons

The site's icon set is IcoFont (icofont.com), a single-colour line and solid set. Icons are licensed CC BY 4.0: credit "Icons by IcoFont (icofont.com)" somewhere on the site, for example in the footer or on a credits page.

This group holds the 21 IcoFont icons the site uses today, plus 9 it needs for common UI (email, social, arrow, menu, search, user). Each file is IcoFont's own SVG on a 1000×1000 grid in a single black ink.

**Using them**

- **On the website:** load IcoFont's stylesheet as the site does (`css/icofont.css`) and write `<i class="icofont-airplane-alt"></i>`. The icon takes the text colour.
- **In components and mockups:** inline the SVG with `fill="currentColor"` and the `tk-ico` class, so it takes the surrounding colour, as the previews do.
- **In Arabic:** mirror directional icons (`long-arrow-right`, `simple-right`) with `transform: scaleX(-1)`.

**Colours and sizes**

- `primary` inside outlined circles (Feature, 50px).
- White on `navy` and on the stats band (28px).
- `primary` beside contact details (16px).
- Never use `logo-aqua` or `sand` for icons.

**What each icon is for**

| Area | Icons |
| --- | --- |
| Airport and project | `airplane-alt`, `building`, `building-alt`, `cement-mix`, `vehicle-dozer`, `barricade`, `ui-network`, `ui-wifi` |
| Services (project page) | `hospital`, `prescription`, `fire-truck`, `police-badge`, `dog`, `hand` |
| Contact | `ui-call`, `ui-head-phone`, `email`, `location-pin`, `google-map`, `wall-clock` |
| Social | `facebook`, `twitter`, `instagram`, `youtube-play` |
| Interface | `rounded-down`, `simple-right`, `long-arrow-right`, `navigation-menu`, `search-1`, `user-alt-7` |
