# Hero

The home page's opening band (`.slider .single-slider`): a full-width project photo set to cover, 600px tall on desktop and 380px on phones. The headline block sits on the left (right in Arabic) across about 7 of 12 columns.

- **Headline:** `hero` style (38/42, weight 400) in `ink`, with the key word ("Karbala") in `primary`. In Arabic, use `ar-hero`.
- **Subtitle:** `hero-subtitle` (20/24, weight 500) in `ink`, the same size at every width.
- **Button:** one dark button ("Learn More") `space-30` below. On phones it spans the full width at 13px.

The preview shows desktop in English, desktop in Arabic, and a 375px phone. The `tk-hero--phone` class forces the phone layout; a real page switches automatically below 768px.

Flag: on phones the site shrinks the headline to 13px, smaller than the 20px subtitle, so the subtitle reads as the title. This is kept to match the site. For new pages, consider keeping the headline at least 20px.

The consumer provides the photo, set as the band's background image. It must be light enough behind the text for `ink` to read at 4.5:1.
