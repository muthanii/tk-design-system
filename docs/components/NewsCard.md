# NewsCard

An item on "News and Updates" (`news.html`, `.blog-item`), three to a row with `space-30` gutters.

- **Card:** a `surface-card` (#f8f9fa) ground, `radius-4` corners, no shadow.
- **Image:** full width at about 290:166.
- **Category tag:** a square `primary` block with white 18px text, padded 8px × `space-24`, inset `space-24`.
- **Body** (padded `space-24`):
  - a meta line: a `primary` IcoFont `user-alt-7` icon and the author in 14.4px `text`;
  - a `news-title` heading (24/28.8, weight 500) in `ink`;
  - the excerpt in 18px `text`;
  - an uppercase "more" link with an IcoFont `long-arrow-right` in `text`, turning `primary` on hover.

The consumer provides the image, category, author, title, excerpt and link. Use real project photography (see the Photography asset group); the preview uses three of those photos.

Flags against the live page:

- The site prints the whole article in the card. Cut excerpts to about three lines.
- The site's tag uses Bootstrap's default blue (#007bff) instead of the brand blue, and leaves a large empty gap under the image. Both are corrected here to `primary` and a tight layout.
- The site shows no date. Add one to the meta line if dates matter.
